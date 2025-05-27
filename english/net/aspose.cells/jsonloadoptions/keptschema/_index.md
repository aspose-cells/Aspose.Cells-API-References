---
title: JsonLoadOptions.KeptSchema
second_title: Aspose.Cells for .NET API Reference
description: JsonLoadOptions property. Indicates whether keeping schema of this json
type: docs
url: /net/aspose.cells/jsonloadoptions/keptschema/
---
## JsonLoadOptions.KeptSchema property

Indicates whether keeping schema of this json.

```csharp
public bool KeptSchema { get; set; }
```

### Remarks

Sometimes we will save the file to JSON after loading JSON file.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyKeptSchemaDemo
    {
        public static void Run()
        {
            // Create JSON layout options
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions
            {
                ArrayAsTable = true,
                ConvertNumericOrDate = true
            };

            // Create sample JSON data
            string jsonData = @"{
                ""schema"": {
                    ""columns"": [
                        {""name"": ""ID"", ""type"": ""number""},
                        {""name"": ""Name"", ""type"": ""string""}
                    ]
                },
                ""data"": [
                    {""ID"": 1, ""Name"": ""John""},
                    {""ID"": 2, ""Name"": ""Jane""}
                ]
            }";

            // Create workbook from JSON with schema preservation
            Workbook workbook = new Workbook();
            JsonUtility.ImportData(jsonData, workbook.Worksheets[0].Cells, 0, 0, layoutOptions);

            // Save the result
            workbook.Save("JsonWithKeptSchema.xlsx");
        }
    }
}
```

### See Also

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


