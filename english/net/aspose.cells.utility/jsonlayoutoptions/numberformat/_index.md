---
title: JsonLayoutOptions.NumberFormat
second_title: Aspose.Cells for .NET API Reference
description: JsonLayoutOptions property. Gets and sets the format of numeric value
type: docs
url: /net/aspose.cells.utility/jsonlayoutoptions/numberformat/
---
## JsonLayoutOptions.NumberFormat property

Gets and sets the format of numeric value.

```csharp
public string NumberFormat { get; set; }
```

### Examples

```csharp
// Called: NumberFormat = "0.00",
public static void JsonLayoutOptions_Property_NumberFormat()
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

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


