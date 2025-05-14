---
title: OoxmlSaveOptions.WpsCompatibility
second_title: Aspose.Cells for .NET API Reference
description: OoxmlSaveOptions property. Indicates whether to make the xls more compatible with WPS
type: docs
url: /net/aspose.cells/ooxmlsaveoptions/wpscompatibility/
---
## OoxmlSaveOptions.WpsCompatibility property

Indicates whether to make the xls more compatible with WPS.

```csharp
public bool WpsCompatibility { get; set; }
```

### Examples

```csharp
// Called: options.WpsCompatibility = true;
public void OoxmlSaveOptions_Property_WpsCompatibility()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    OoxmlSaveOptions options = new OoxmlSaveOptions();
    options.WpsCompatibility = true;
    workbook.Save(Constants.destPath + "example.xlsx", options);
    Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + "example.xlsx",
      "xl/cellImages.xml", new string[] { "a:off x=\"3777615\"" }, true));
}
```

### See Also

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


