---
title: OdsSaveOptions.OdsSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: OdsSaveOptions constructor. Creates the options of saving ods file
type: docs
url: /net/aspose.cells/odssaveoptions/odssaveoptions/
---
## OdsSaveOptions() {#constructor}

Creates the options of saving ods file.

```csharp
public OdsSaveOptions()
```

### Examples

```csharp
// Called: OdsSaveOptions saveOptions = new OdsSaveOptions();
public void OdsSaveOptions_Constructor()
{
    Style style = null;
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    OdsSaveOptions saveOptions = new OdsSaveOptions();
    saveOptions.GeneratorType = Aspose.Cells.Ods.OdsGeneratorType.LibreOffice;
            
    workbook.Save(Constants.destPath + "example.ods", saveOptions);
    workbook = new Workbook(Constants.destPath + "example.ods");
    style = workbook.Worksheets[0].Cells["B2"].GetStyle();
    Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Medium);
    style = workbook.Worksheets[0].Cells["B4"].GetStyle();
    Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Thick);
    style = workbook.Worksheets[0].Cells["B7"].GetStyle();
    Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Double);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    style = workbook.Worksheets[0].Cells["B2"].GetStyle();
    Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Medium);
    style = workbook.Worksheets[0].Cells["B4"].GetStyle();
    Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Thick);
    style = workbook.Worksheets[0].Cells["B7"].GetStyle();
    Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Double);
}
```

### See Also

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsSaveOptions(SaveFormat) {#constructor_1}

Creates the options of saving ods file.

```csharp
public OdsSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be Ods, Ots, Fods or Sxc, otherwise the saved format will be set as Ods automatically. |

### See Also

* enum [SaveFormat](../../saveformat/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


