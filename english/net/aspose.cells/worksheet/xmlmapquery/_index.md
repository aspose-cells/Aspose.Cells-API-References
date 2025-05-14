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
// Called: ArrayList cellAreaList = wb.Worksheets[0].XmlMapQuery("/ns1:Contract_Revenue_FTS_-_V3/ns1:COLUMN_HEADINGS/ns1:CUSTOMER_ACCOUNT_REF_NO",
public void Worksheet_Method_XmlMapQuery()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual("D:\\ProjectsMA.Net\\Posey\\data\\xml.xml", wb.DataConnections[0].ConnectionFile);

    wb.ImportXml(Constants.sourcePath + "example.xml", "Sheet1", 0, 0);

    ArrayList cellAreaList = wb.Worksheets[0].XmlMapQuery("/ns1:Contract_Revenue_FTS_-_V3/ns1:COLUMN_HEADINGS/ns1:CUSTOMER_ACCOUNT_REF_NO",
        wb.Worksheets.XmlMaps[0]);

    Assert.AreEqual(6, ((CellArea)cellAreaList[0]).StartRow);
    Assert.AreEqual("Account No.", wb.Worksheets[0].Cells["A7"].StringValue);

}
```

### See Also

* class [XmlMap](../../xmlmap/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


