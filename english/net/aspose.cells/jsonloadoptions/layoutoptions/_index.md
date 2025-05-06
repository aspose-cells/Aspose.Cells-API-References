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
public static void Property_LayoutOptions()
        {
            // Create an instance of JsonLoadOptions
            JsonLoadOptions jsonLoadOptions = new JsonLoadOptions
            {
                StartCell = &quot;A1&quot;,
                MultipleWorksheets = true,
                KeptSchema = true,
                LayoutOptions = new JsonLayoutOptions
                {
                    ArrayAsTable = true,
                    IgnoreNull = false,
                    IgnoreTitle = false,
                    ConvertNumericOrDate = true,
                    NumberFormat = &quot;0.00&quot;,
                    DateFormat = &quot;yyyy-MM-dd&quot;
                }
            };

            // Load JSON data into a Workbook
            string jsonFilePath = &quot;JsonLoadOptionsExample_data.json&quot;;
            Workbook workbook = new Workbook(jsonFilePath, jsonLoadOptions);

            // Save the workbook to an Excel file
            workbook.Save(&quot;JsonLoadOptionsExample.xlsx&quot;);
        }
```

### See Also

* class [JsonLayoutOptions](../../../aspose.cells.utility/jsonlayoutoptions/)
* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


