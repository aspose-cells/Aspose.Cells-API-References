---
title: XmlMapCollection.Clear
second_title: Aspose.Cells for .NET API Reference
description: XmlMapCollection method. Removes all XmlMaps
type: docs
url: /net/aspose.cells/xmlmapcollection/clear/
---
## XmlMapCollection.Clear method

Removes all XmlMaps.

```csharp
public void Clear()
```

### Examples

```csharp
// Called: xmlMaps.Clear();
public static void Method_Clear()
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

* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


