---
title: JsonSaveOptions.ToExcelStruct
second_title: Aspose.Cells for .NET API Reference
description: JsonSaveOptions property. Indicates whether converting to json struct of the Excel file
type: docs
url: /net/aspose.cells/jsonsaveoptions/toexcelstruct/
---
## JsonSaveOptions.ToExcelStruct property

Indicates whether converting to json struct of the Excel file.

```csharp
public bool ToExcelStruct { get; set; }
```

### Remarks

Only for converting range to JSON.

### Examples

```csharp
// Called: saveOptions.ToExcelStruct = true;
[Test]
        public void Property_ToExcelStruct()
        {
            Workbook workbook = new Workbook();
            Workbook wb = new Workbook(Constants.sourcePath + "CellsNet55039.xlsx");
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ToExcelStruct = true;
            wb.Save(Constants.destPath + "CellsNet55039.json", saveOptions);
            string t1 = File.ReadAllText(Constants.destPath + "CellsNet55039.json");
            string t2 = File.ReadAllText(Constants.sourcePath + "CellsNet55039.json");
            Assert.AreEqual(t1, t2);

        }
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


