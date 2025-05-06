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
// Called: StartCell = &amp;quot;A1&amp;quot;,
public static void Property_StartCell()
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

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


