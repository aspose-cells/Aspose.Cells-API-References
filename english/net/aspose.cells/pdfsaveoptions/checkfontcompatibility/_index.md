---
title: CheckFontCompatibility
second_title: Aspose.Cells for .NET API Reference
description: Indicates whether to check font compatibility for every character in text.
type: docs
weight: 50
url: /net/aspose.cells/pdfsaveoptions/checkfontcompatibility/
---
## PdfSaveOptions.CheckFontCompatibility property

Indicates whether to check font compatibility for every character in text.

```csharp
public bool CheckFontCompatibility { get; set; }
```

### Remarks

The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;

### See Also

* class [PdfSaveOptions](../../pdfsaveoptions)
* namespace [Aspose.Cells](../../pdfsaveoptions)
* assembly [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
