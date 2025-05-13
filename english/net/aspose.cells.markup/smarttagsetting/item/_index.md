---
title: SmartTagSetting.Item
second_title: Aspose.Cells for .NET API Reference
description: SmartTagSetting property. Gets a SmartTagCollection object by the index
type: docs
url: /net/aspose.cells.markup/smarttagsetting/item/
---
## SmartTagSetting indexer (1 of 3)

Gets a [`SmartTagCollection`](../../smarttagcollection/) object by the index.

```csharp
public SmartTagCollection this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index of the [`SmartTagCollection`](../../smarttagcollection/) object in the list. |

### Examples

```csharp
// Called: SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
public static void SmartTagSetting_Property_Item()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells["A1"].PutValue("Aspose");
            sheet.Cells["A2"].PutValue("Cells");

            // Access the SmartTagSetting of the worksheet
            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;

            // Add a smart tag to cell A1
            int smartTagIndex = smartTagSetting.Add(0, 0); // A1 is at row 0, column 0
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            // Add properties to the smart tag
            smartTags.Add("http://docs.aspose.com", "docs");
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            // Add properties to the smart tag
            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Description", "Aspose.Cells SmartTag");

            // Save the workbook
            workbook.Save("SmartTagPropertyDemo.xlsx");

            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
```

### See Also

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (2 of 3)

Gets the [`SmartTagCollection`](../../smarttagcollection/) object of the cell.

```csharp
public SmartTagCollection this[int row, int column] { get; }
```

| Parameter | Description |
| --- | --- |
| row | The row index of the cell. |
| column | The column index of the cell |

### Return Value

Returns the [`SmartTagCollection`](../../smarttagcollection/) object of the cell. Returns null if there is no any smart tags on the cell.

### Examples

```csharp
// Called: SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
public static void SmartTagSetting_Property_Item()
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

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (3 of 3)

Gets the [`SmartTagCollection`](../../smarttagcollection/) object of the cell.

```csharp
public SmartTagCollection this[string cellName] { get; }
```

| Parameter | Description |
| --- | --- |
| cellName | The name of the cell. |

### Return Value

Returns the [`SmartTagCollection`](../../smarttagcollection/) object of the cell. Returns null if there is no any smart tags on the cell.

### See Also

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


