---
title: SmartTagCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: SmartTagCollection method. Adds a smart tag
type: docs
url: /net/aspose.cells.markup/smarttagcollection/add/
---
## SmartTagCollection.Add method

Adds a smart tag.

```csharp
public int Add(string uri, string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| uri | String | Specifies the namespace URI of the smart tag |
| name | String | Specifies the name of the smart tag. |

### Return Value

The index of smart tag in the list.

### Examples

```csharp
// Called: int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");
public static void Method_String_()
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

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


