---
title: Range.ToJson
second_title: Aspose.Cells for .NET API Reference
description: Range method. Convert the range to JSON value
type: docs
url: /net/aspose.cells/range/tojson/
---
## Range.ToJson method

Convert the range to JSON value.

```csharp
public string ToJson(JsonSaveOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | JsonSaveOptions | The options of converting |

### Examples

```csharp
// Called: string json = range.ToJson(saveOptions);
[Test]
        public void Method_JsonSaveOptions_()
        {
            Workbook book = new Workbook(Constants.sourcePath + "CELLSNET55579.xlsx");
            Aspose.Cells.Range range = book.Worksheets[0].Cells.CreateRange("A1:B2");

            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;
            string json = range.ToJson(saveOptions);
            Assert.IsTrue(json.IndexOf("\"cell\" :") > 0);
        }
```

### See Also

* class [JsonSaveOptions](../../jsonsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


