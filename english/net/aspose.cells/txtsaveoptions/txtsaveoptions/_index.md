---
title: TxtSaveOptions.TxtSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions constructor. Creates text file save options
type: docs
url: /net/aspose.cells/txtsaveoptions/txtsaveoptions/
---
## TxtSaveOptions() {#constructor}

Creates text file save options.

```csharp
public TxtSaveOptions()
```

### Examples

```csharp
// Called: TxtSaveOptions saveOptions = new TxtSaveOptions();
[Test, Ignore("Not ready to test this yet")]
        public void TxtSaveOptions_Constructor()
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

---

## TxtSaveOptions(SaveFormat) {#constructor_1}

Creates text file save options.

```csharp
public TxtSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be Csv or Tsv, otherwise the saved format will be set as Csv automatically. |

### See Also

* enum [SaveFormat](../../saveformat/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


