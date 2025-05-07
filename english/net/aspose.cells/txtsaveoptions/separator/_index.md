---
title: TxtSaveOptions.Separator
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions property. Gets and sets char Delimiter of text file
type: docs
url: /net/aspose.cells/txtsaveoptions/separator/
---
## TxtSaveOptions.Separator property

Gets and sets char Delimiter of text file.

```csharp
public char Separator { get; set; }
```

### Examples

```csharp
// Called: saveOptions.Separator = ',';
[Test, Ignore("Not ready to test this yet")]
        public void Property_Separator()
        {
            string FileName = Constants.sourcePath + "TestWorkbook\\Book1.xls";
            Workbook workbook = new Workbook(FileName);
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.Separator = ',';
            workbook.Save(Constants.destPath + "testSave.CSV", saveOptions);

            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = ',';
            workbook = new Workbook(Constants.destPath + "testSave.CSV", loadOptions);
            Assert.AreEqual(1, workbook.Worksheets.Count, "workbook.Worksheets.Count");
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;
            Assert.AreEqual("Tabelle1", cells[0, 0].StringValue);
            Assert.AreEqual("", cells[1, 1].StringValue);
            Assert.AreEqual("3", cells[2, 1].IntValue);
        }
```

### See Also

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


