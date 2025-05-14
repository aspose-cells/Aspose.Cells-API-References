---
title: CustomPropertyCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: CustomPropertyCollection property. Gets the custom property by the specific index
type: docs
url: /net/aspose.cells.properties/custompropertycollection/item/
---
## CustomPropertyCollection indexer (1 of 2)

Gets the custom property by the specific index.

```csharp
public CustomProperty this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

The custom property

### Examples

```csharp
// Called: CustomProperty property = customProperties[i];
public static void CustomPropertyCollection_Property_Item()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Access the CustomProperties collection
            CustomPropertyCollection customProperties = sheet.CustomProperties;

            // Add custom properties
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");
            customProperties.Add("LastModified", DateTime.Now.ToString());

            // Access and display custom properties
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            // Save the workbook
            workbook.Save("CustomPropertyExample.xlsx");
            workbook.Save("CustomPropertyExample.pdf");
        }
```

### See Also

* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## CustomPropertyCollection indexer (2 of 2)

Gets the custom property by the property name.

```csharp
public CustomProperty this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The property name. |

### Return Value

The custom property

### Examples

```csharp
// Called: Assert.AreEqual(o1.CustomProperties["COR_ResultSet"].Value, o2.CustomProperties["COR_ResultSet"].Value);
public void CustomPropertyCollection_Property_Item()
{
    var excelWorkbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var o1 = excelWorkbook.Worksheets[0];


    String filePath = Constants.sourcePath + "example.xls";
    Workbook xlsWorkbook = new Workbook(filePath);
    var o2 = xlsWorkbook.Worksheets[0];

    Assert.AreEqual(o1.CustomProperties["COR_Report"].Value, o2.CustomProperties["COR_Report"].Value);
    //{
    //    Console.WriteLine("COR_Report is equal in both files.");
    //}

    Assert.AreEqual(o1.CustomProperties["COR_ResultSet"].Value, o2.CustomProperties["COR_ResultSet"].Value);
    //{
    //    Console.WriteLine("COR_ResultSet is equal in both files.");
    //} 

}
```

### See Also

* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


