---
title: JsonLoadOptions.LayoutOptions
second_title: Aspose.Cells for .NET API Reference
description: JsonLoadOptions property. The options of import json
type: docs
url: /net/aspose.cells/jsonloadoptions/layoutoptions/
---
## JsonLoadOptions.LayoutOptions property

The options of import json.

```csharp
public JsonLayoutOptions LayoutOptions { get; set; }
```

### Examples

```csharp
// Called: LayoutOptions = new JsonLayoutOptions
public static void JsonLoadOptions_Property_LayoutOptions()
        {
            // Create an instance of JsonLoadOptions
            JsonLoadOptions jsonLoadOptions = new JsonLoadOptions
            {
                StartCell = "A1",
                MultipleWorksheets = true,
                KeptSchema = true,
                LayoutOptions = new JsonLayoutOptions
                {
                    ArrayAsTable = true,
                    IgnoreNull = false,
                    IgnoreTitle = false,
                    ConvertNumericOrDate = true,
                    NumberFormat = "0.00",
                    DateFormat = "yyyy-MM-dd"
                }
            };

            // Load JSON data into a Workbook
            string jsonFilePath = "JsonLoadOptionsExample_data.json";
            Workbook workbook = new Workbook(jsonFilePath, jsonLoadOptions);

            // Save the workbook to an Excel file
            workbook.Save("JsonLoadOptionsExample.xlsx");
        }
```

### See Also

* class [JsonLayoutOptions](../../../aspose.cells.utility/jsonlayoutoptions/)
* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


