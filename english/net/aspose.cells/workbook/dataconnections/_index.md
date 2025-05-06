---
title: Workbook.DataConnections
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets the ExternalConnection collection
type: docs
url: /net/aspose.cells/workbook/dataconnections/
---
## Workbook.DataConnections property

Gets the [`ExternalConnection`](../../../aspose.cells.externalconnections/externalconnection/) collection.

```csharp
public ExternalConnectionCollection DataConnections { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;D:\\ProjectsMA.Net\\Posey\\data\\xml.xml&amp;quot;, wb.DataConnections[0].ConnectionFile);
[Test]
        public void Property_DataConnections()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-53381/Template.xlsx&quot;);
            Assert.AreEqual(&quot;D:\\ProjectsMA.Net\\Posey\\data\\xml.xml&quot;, wb.DataConnections[0].ConnectionFile);

            wb.ImportXml(Constants.sourcePath + &quot;CELLSNET-53381/xml.xml&quot;, &quot;Sheet1&quot;, 0, 0);

            ArrayList cellAreaList = wb.Worksheets[0].XmlMapQuery(&quot;/ns1:Contract_Revenue_FTS_-_V3/ns1:COLUMN_HEADINGS/ns1:CUSTOMER_ACCOUNT_REF_NO&quot;,
                wb.Worksheets.XmlMaps[0]);

            Assert.AreEqual(6, ((CellArea)cellAreaList[0]).StartRow);
            Assert.AreEqual(&quot;Account No.&quot;, wb.Worksheets[0].Cells[&quot;A7&quot;].StringValue);

        }
```

### See Also

* class [ExternalConnectionCollection](../../../aspose.cells.externalconnections/externalconnectioncollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


