---
title: SmartTagSetting.Add
second_title: Aspose.Cells for .NET API Reference
description: SmartTagSetting method. Adds a SmartTagCollection object to a cell
type: docs
url: /net/aspose.cells.markup/smarttagsetting/add/
---
## Add(int, int) {#add}

Adds a [`SmartTagCollection`](../../smarttagcollection/) object to a cell.

```csharp
public int Add(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row of the cell. |
| column | Int32 | The column of the cell. |

### Return Value

Returns index of a [`SmartTagCollection`](../../smarttagcollection/) object in the worksheet.

### Examples

```csharp
// Called: int smartTagIndex = smartTagSetting.Add(0, 0); // Adding smart tag to cell A1
public static void SmartTagSetting_Method_Add()
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

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Add a cell smart tags.

```csharp
public int Add(string cellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | The name of the cell. |

### See Also

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


