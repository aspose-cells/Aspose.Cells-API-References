---
title: JsonLoadOptions.StartCell
second_title: Aspose.Cells for .NET API Reference
description: JsonLoadOptions property. Gets and sets the start cell
type: docs
url: /net/aspose.cells/jsonloadoptions/startcell/
---
## JsonLoadOptions.StartCell property

Gets and sets the start cell.

```csharp
public string StartCell { get; set; }
```

### Examples

```csharp
// Called: StartCell = "A1",
public static void Property_StartCell()
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

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


