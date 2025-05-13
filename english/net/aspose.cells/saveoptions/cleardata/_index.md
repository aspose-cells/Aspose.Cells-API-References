---
title: SaveOptions.ClearData
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. Make the workbook empty after saving the file
type: docs
url: /net/aspose.cells/saveoptions/cleardata/
---
## SaveOptions.ClearData property

Make the workbook empty after saving the file.

```csharp
public bool ClearData { get; set; }
```

### Examples

```csharp
// Called: txtSaveOptions.ClearData = false;
public void SaveOptions_Property_ClearData()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "TestWorkbook\\Book1.xls");
    TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
    txtSaveOptions.TrimLeadingBlankRowAndColumn = false;
    txtSaveOptions.Separator = ',';
    txtSaveOptions.ClearData = false;
            
    workbook.Save(Constants.destPath + "testSave.CSV", txtSaveOptions);
    LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
    workbook = new Workbook(Constants.destPath + "testSave.CSV", loadOptions);
    Cells cells = workbook.Worksheets[0].Cells;
    Assert.AreEqual("Tabelle1", cells[1, 1].StringValue);
    Assert.AreEqual(3, cells[3, 2].IntValue);
}
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


