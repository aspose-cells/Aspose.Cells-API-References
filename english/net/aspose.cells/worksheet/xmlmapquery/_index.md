---
title: Worksheet.XmlMapQuery
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Query cell areas that mapped/linked to the specific path of xml map
type: docs
url: /net/aspose.cells/worksheet/xmlmapquery/
---
## Worksheet.XmlMapQuery method

Query cell areas that mapped/linked to the specific path of xml map.

```csharp
public ArrayList XmlMapQuery(string path, XmlMap xmlMap)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | xml element path |
| xmlMap | XmlMap | Specify an xml map if you want to query for the specific path within a specific map |

### Return Value

[`CellArea`](../../cellarea/) list that mapped/linked to the specific path of xml map, an empty list is returned if nothing is mapped/linked.

### Examples

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodXmlMapQueryWithStringXmlMapDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            
            // Add a worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Create a sample XML map
            string xml = @"<?xml version='1.0' encoding='UTF-8'?>
                <ns1:Root xmlns:ns1='http://example.com'>
                    <ns1:Data>
                        <ns1:Item>Value1</ns1:Item>
                    </ns1:Data>
                </ns1:Root>";
            
            // Import XML to create the map
            workbook.ImportXml(xml, "Sheet1", 0, 0);
            
            // Get the XML map
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[0];
            
            // Query the XML map
            ArrayList cellAreas = worksheet.XmlMapQuery("/ns1:Root/ns1:Data/ns1:Item", xmlMap);
            
            // Output results
            if (cellAreas.Count > 0)
            {
                CellArea area = (CellArea)cellAreas[0];
                Console.WriteLine($"Found data at row {area.StartRow}, column {area.StartColumn}");
                Console.WriteLine($"Cell value: {worksheet.Cells[area.StartRow, area.StartColumn].StringValue}");
            }
        }
    }
}
```

### See Also

* class [XmlMap](../../xmlmap/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


