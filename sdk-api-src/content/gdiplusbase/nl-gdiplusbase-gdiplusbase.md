---
UID: NL:gdiplusbase.GdiplusBase
title: GdiplusBase (gdiplusbase.h)
description: The GdiplusBase class provides memory allocation and deallocation for GDI+ objects. GdiplusBase serves as a base class for all other GDI+ classes, so you never need to create an instance of GdiplusBase.
old-location: gdiplus\_gdiplus_CLASS_GdiplusBase_Class.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\gdiplusbase.htm
ms.date: 12/05/2018
ms.keywords: GdiplusBase, GdiplusBase class [GDI+], GdiplusBase class [GDI+],described, _gdiplus_CLASS_GdiplusBase_Class, gdiplus._gdiplus_CLASS_GdiplusBase_Class, gdiplusbase/GdiplusBase
f1_keywords:
- gdiplusbase/GdiplusBase
dev_langs:
- c++
req.header: gdiplusbase.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
- COM
api_location:
- gdiplusbase.h
api_name:
- GdiplusBase
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# GdiplusBase class


## -description


The <b>GdiplusBase</b> class provides memory allocation and deallocation for GDI+ objects. <b>GdiplusBase</b> serves as a base class for all other GDI+ classes, so you never need to create an instance of <b>GdiplusBase</b>.

<b xmlns:loc="http://microsoft.com/wdcml/l10n">GdiplusBase</b> has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul><h3><a id="methods"></a>Methods</h3>The <b>GdiplusBase</b> class has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/gdiplusbase/nf-gdiplusbase-gdiplusbase-operatordelete">GdiplusBase::operator delete</a>
</td>
<td align="left" width="63%">
The <a href="https://docs.microsoft.com/windows/desktop/api/gdiplusbase/nf-gdiplusbase-gdiplusbase-operatordelete">GdiplusBase::operator delete</a> method deallocates memory for one GDI+ object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/gdiplusbase/nf-gdiplusbase-gdiplusbase-operatordelete%5B%5D">GdiplusBase::operator delete[]</a>
</td>
<td align="left" width="63%">
The 
		xref rid="_gdiplus_CLASS_GdiplusBase_operator_delete_bracket_in_pVoid_" qualify="0"/&gt; 
		method deallocates memory for an array of GDI+ 
		objects.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/gdiplusbase/nf-gdiplusbase-gdiplusbase-operatornew">GdiplusBase::operator new</a>
</td>
<td align="left" width="63%">
The <a href="https://docs.microsoft.com/windows/desktop/api/gdiplusbase/nf-gdiplusbase-gdiplusbase-operatornew">GdiplusBase::operator new</a> method allocates memory for one GDI+ object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/gdiplusbase/nf-gdiplusbase-gdiplusbase-operatornew%5B%5D">GdiplusBase::operator new[]</a>
</td>
<td align="left" width="63%">
The <a href="https://docs.microsoft.com/windows/desktop/api/gdiplusbase/nf-gdiplusbase-gdiplusbase-operatornew%5B%5D">GdiplusBase::operator new[]</a> method allocates memory for an array of GDI+ objects.

</td>
</tr>
</table> 

