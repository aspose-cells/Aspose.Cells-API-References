---
title: TxtSaveOptions.TrimLeadingBlankRowAndColumn
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions property. Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true
type: docs
url: /net/aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/
---
## TxtSaveOptions.TrimLeadingBlankRowAndColumn property

Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true.

```csharp
public bool TrimLeadingBlankRowAndColumn { get; set; }
```

### Remarks

Same with the rule in ms excel, a row/column will not be taken as blank if it has custom style, even if it contains no cell data. When saving with LightCells mode, this option takes no effect. User should control the output range by the implementation of [`LightCellsDataProvider`](../lightcellsdataprovider/) or by speicifing [`ExportArea`](../exportarea/)

### Examples

```csharp
// Called: saveOptions.TrimLeadingBlankRowAndColumn = false;
public void TxtSaveOptions_Property_TrimLeadingBlankRowAndColumn()
{
    string FileName = Constants.sourcePath + "TestWorkbook\\Book1.xls";
    Workbook workbook = new Workbook(FileName);
    TxtSaveOptions saveOptions = new TxtSaveOptions();
    saveOptions.TrimLeadingBlankRowAndColumn = false;
    saveOptions.SeparatorString = "";
    workbook.Save(Constants.destPath + "testSave.CSV", saveOptions);

    TxtLoadOptions loadOptions = new TxtLoadOptions();
    saveOptions.SeparatorString = "";
    workbook = new Workbook(Constants.destPath + "testSave.CSV", loadOptions);
    Cells cells = workbook.Worksheets[0].Cells;
    Assert.AreEqual("Tabelle1", cells[1, 0].StringValue);
    Assert.AreEqual(3, cells[3, 0].IntValue);
}
```

### See Also

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


