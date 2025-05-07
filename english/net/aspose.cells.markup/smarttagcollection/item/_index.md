---
title: SmartTagCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: SmartTagCollection property. Gets a SmartTag object at the specific index
type: docs
url: /net/aspose.cells.markup/smarttagcollection/item/
---
## SmartTagCollection indexer

Gets a [`SmartTag`](../../smarttag/) object at the specific index

```csharp
public SmartTag this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

returns a [`SmartTag`](../../smarttag/) object.

### Examples

```csharp
// Called: SmartTag smartTag = smartTags[0];
public static void Property_Int32_()
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

* class [SmartTag](../../smarttag/)
* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


