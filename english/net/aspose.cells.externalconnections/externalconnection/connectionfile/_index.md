---
title: ExternalConnection.ConnectionFile
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Gets the connection file
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/connectionfile/
---
## ExternalConnection.ConnectionFile property

Gets the connection file.

```csharp
public virtual string ConnectionFile { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("D:\\ProjectsMA.Net\\Posey\\data\\xml.xml", wb.DataConnections[0].ConnectionFile);
[Test]
        public void Property_ConnectionFile()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSNET-53381/Template.xlsx");
            Assert.AreEqual("D:\\ProjectsMA.Net\\Posey\\data\\xml.xml", wb.DataConnections[0].ConnectionFile);

            wb.ImportXml(Constants.sourcePath + "CELLSNET-53381/xml.xml", "Sheet1", 0, 0);

            ArrayList cellAreaList = wb.Worksheets[0].XmlMapQuery("/ns1:Contract_Revenue_FTS_-_V3/ns1:COLUMN_HEADINGS/ns1:CUSTOMER_ACCOUNT_REF_NO",
                wb.Worksheets.XmlMaps[0]);

            Assert.AreEqual(6, ((CellArea)cellAreaList[0]).StartRow);
            Assert.AreEqual("Account No.", wb.Worksheets[0].Cells["A7"].StringValue);

        }
```

### See Also

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


