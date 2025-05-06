---
title: JsonLayoutOptions.JsonLayoutOptions
second_title: Aspose.Cells for .NET API Reference
description: JsonLayoutOptions constructor. Constructor of loading JSON layout options
type: docs
url: /net/aspose.cells.utility/jsonlayoutoptions/jsonlayoutoptions/
---
## JsonLayoutOptions constructor

Constructor of loading JSON layout options.

```csharp
public JsonLayoutOptions()
```

### Examples

```csharp
// Called: JsonLayoutOptions options = new JsonLayoutOptions();
public void JsonLayoutOptions_Constructor()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            string json = File.ReadAllText(Constants.sourcePath + &quot;CELLSNET46553.bd5&quot;);
             JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            options.IgnoreNull = true;

            options.IgnoreTitle = true;
            options.NumberFormat = &quot;$0.00&quot;;
            options.ConvertNumericOrDate = true;
            JsonUtility.ImportData(json, cells, 0, 0, options);
            Assert.AreEqual(cells[&quot;E2&quot;].StringValue, &quot;$500.00&quot;);
            Assert.AreEqual(&quot;sun1.opacity = (sun1.opacity / 100) * 90;&quot;, cells[&quot;R2&quot;].StringValue);
            Assert.AreEqual(&quot;$36.00&quot;, cells[&quot;L2&quot;].StringValue);
            workbook.Save(Constants.destPath + &quot;CELLSNET46553.xlsx&quot;);
        }
```

### See Also

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


