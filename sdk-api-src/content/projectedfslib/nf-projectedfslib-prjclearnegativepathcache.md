---
UID: NF:projectedfslib.PrjClearNegativePathCache
title: PrjClearNegativePathCache function (projectedfslib.h)
description: Purges the virtualization instance's negative path cache, if it is active.
old-location: projfs\prjclearnegativepathcache.htm
tech.root: ProjFS
ms.assetid: 90E37386-C647-476C-A53D-C479411DF8F9
ms.date: 12/05/2018
ms.keywords: PrjClearNegativePathCache, PrjClearNegativePathCache function, ProjFS.prjclearnegativepathcache, projectedfslib/PrjClearNegativePathCache
f1_keywords:
- projectedfslib/PrjClearNegativePathCache
dev_langs:
- c++
req.header: projectedfslib.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1809 [desktop apps only]
req.target-min-winversvr: Windows Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- HeaderDef
api_location:
- projectedfslib.h
api_name:
- PrjClearNegativePathCache
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: RS5, 19H1
---

# PrjClearNegativePathCache function


## -description


Purges the virtualization instance's negative path cache, if it is active.


## -parameters




### -param namespaceVirtualizationContext [in]

Opaque handle for the virtualization instance.


### -param totalEntryNumber [out, optional]

Optional pointer to a variable that receives the number of paths that were in the cache before it was purged.


## -returns



If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



If the negative path cache is active, then if the provider indicates that a file path does not exist by returning HRESULT_FROM_WIN32(ERROR_FILE_NOT_FOUND) from its <a href="https://docs.microsoft.com/windows/desktop/api/projectedfslib/nc-projectedfslib-prj_get_placeholder_info_cb">PRJ_GET_PLACEHOLDER_INFO_CB</a> callback, ProjFS will fail subsequent opens of that path without calling the <a href="https://docs.microsoft.com/windows/desktop/api/projectedfslib/nc-projectedfslib-prj_get_placeholder_info_cb">PRJ_GET_PLACEHOLDER_INFO_CB</a> callback again. This helps improve performance of virtualization instances that host workloads that frequently probe for the presence of a file by trying to open it. 


To resume receiving the <a href="https://docs.microsoft.com/windows/desktop/api/projectedfslib/nc-projectedfslib-prj_get_placeholder_info_cb">PRJ_GET_PLACEHOLDER_INFO_CB</a> callback for paths the provider has indicated do not exist, the provider must call this routine.



