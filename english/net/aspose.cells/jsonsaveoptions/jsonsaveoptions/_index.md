---
title: JsonSaveOptions.JsonSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: JsonSaveOptions constructor. Creates options for saving json file
type: docs
url: /net/aspose.cells/jsonsaveoptions/jsonsaveoptions/
---
## JsonSaveOptions constructor

Creates options for saving json file.

```csharp
public JsonSaveOptions()
```

### Examples

```csharp
// Called: JsonSaveOptions saveOptions = new JsonSaveOptions();
[Test]
        public void JsonSaveOptions_Constructor()
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


