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
// Called: ArrayList areas = sheet.XmlMapQuery(xPath, xmlMap);
[Test]
        public void Method_XmlMap_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-45748/XmlMaps-1.xlsm&quot;);
            Worksheet sheet = wb.Worksheets[0];
            XmlMap xmlMap = wb.Worksheets.XmlMaps[0];

            string[] xPaths = new string[]
            {
                &quot;/root/row/FIELD1&quot;,
                &quot;/root/row/FIELD2&quot;,
                &quot;/root/row/FIELD3&quot;,
                &quot;/root/row/FIELD4&quot;,
                &quot;/root&quot;,
                &quot;/root/row&quot;,
            };

            string[] expectedAreas = new string[]
            {
                &quot;A1&quot;,
                &quot;B2&quot;,
                &quot;&quot;,
                &quot;C3&quot;,
                &quot;A1,B2,C3,D4,E5,F6&quot;,
                &quot;A1,B2,C3,D4,E5,F6&quot;,
            };

            for (int i = 0; i &lt; xPaths.Length; i++)
            {
                string xPath = xPaths[i];
                ArrayList areas = sheet.XmlMapQuery(xPath, xmlMap);
                Assert.AreEqual(expectedAreas[i], CellAreasToString(areas));
            }
        }
```

### See Also

* class [XmlMap](../../xmlmap/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


