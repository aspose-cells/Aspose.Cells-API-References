---
title: Worksheet.SmartTagSetting
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets all SmartTagCollection objects of the worksheet
type: docs
url: /net/aspose.cells/worksheet/smarttagsetting/
---
## Worksheet.SmartTagSetting property

Gets all [`SmartTagCollection`](../../../aspose.cells.markup/smarttagcollection/) objects of the worksheet.

```csharp
public SmartTagSetting SmartTagSetting { get; }
```

### Examples

```csharp
// Called: SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
public static void Worksheet_Property_SmartTagSetting()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a smart tag to a specific cell
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0); // Adding smart tag to cell A1

            // Access the SmartTagCollection for the cell
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];

            // Add a smart tag to the collection
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            // Set the capacity of the smart tag setting
            smartTagSetting.Capacity = 10;

            // Print the count of smart tags
            Console.WriteLine("Total Smart Tags: " + smartTagSetting.Count);

            // Save the workbook
            workbook.Save("SmartTagSettingExample.xlsx");

            return;
        }
```

### See Also

* class [SmartTagSetting](../../../aspose.cells.markup/smarttagsetting/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


