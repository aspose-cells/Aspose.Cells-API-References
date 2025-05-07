---
title: TxtSaveOptions.SeparatorString
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions property. Gets and sets a string value as separator
type: docs
url: /net/aspose.cells/txtsaveoptions/separatorstring/
---
## TxtSaveOptions.SeparatorString property

Gets and sets a string value as separator.

```csharp
public string SeparatorString { get; set; }
```

### Examples

```csharp
// Called: saveOptions.SeparatorString = ",";
[Test]
        public void Property_SeparatorString()
        {
            string FileName = Constants.sourcePath + "TestWorkbook\\Book1.xls";
            Workbook workbook = new Workbook(FileName);
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.TrimLeadingBlankRowAndColumn = false;
            saveOptions.SeparatorString = ",";
            workbook.Save(Constants.destPath + "testSave.CSV", saveOptions);

            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.SeparatorString = ",";
            workbook = new Workbook(Constants.destPath + "testSave.CSV", loadOptions);
            Cells cells = workbook.Worksheets[0].Cells;
            Assert.AreEqual("Tabelle1", cells[1, 1].StringValue);
            Assert.AreEqual(3, cells[3, 2].IntValue);
        }
```

### See Also

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


