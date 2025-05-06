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
// Called: string json = r.ToJson(null);
[Test]
        public void Method_JsonSaveOptions_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET55578.xlsx&quot;);
            //A1:J25
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range r = cells.CreateRange(&quot;A1:J25&quot;);
            byte[] data = r.ToImage(null);

            byte[] htmlData = r.ToHtml(null);
            string json = r.ToJson(null);
        }
```

### See Also

* class [JsonSaveOptions](../../jsonsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


