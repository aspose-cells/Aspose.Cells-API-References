---
title: XmlMapCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: XmlMapCollection property. Gets the xml map by the specific index
type: docs
url: /net/aspose.cells/xmlmapcollection/item/
---
## XmlMapCollection indexer

Gets the xml map by the specific index.

```csharp
public XmlMap this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

The xml map

### Examples

```csharp
// Called: XmlMap xmlMap = xmlMaps[xmlMapIndex];
public static void Property_Int32_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the XmlMapCollection from the workbook
            XmlMapCollection xmlMaps = workbook.Worksheets.XmlMaps;

            // Add a new XmlMap to the collection
            int xmlMapIndex = xmlMaps.Add("XmlMapCollectionExample.xsd");

            // Access the newly added XmlMap
            XmlMap xmlMap = xmlMaps[xmlMapIndex];

            // Display the count of XmlMaps in the collection
            Console.WriteLine("Number of XmlMaps: " + xmlMaps.Count);

            // Set the capacity of the XmlMapCollection
            xmlMaps.Capacity = 10;

            // Clear all XmlMaps from the collection
            xmlMaps.Clear();

            // Save the workbook
            workbook.Save("XmlMapCollectionExample.xlsx");

            return;
        }
```

### See Also

* class [XmlMap](../../xmlmap/)
* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


