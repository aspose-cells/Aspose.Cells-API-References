---
title: DBConnection.ConnectionString
second_title: Aspose.Cells for .NET API Reference
description: DBConnection property. The connection information string is used to make contact with an OLE DB or ODBC data source
type: docs
url: /net/aspose.cells.externalconnections/dbconnection/connectionstring/
---
## DBConnection.ConnectionString property

The connection information string is used to make contact with an OLE DB or ODBC data source.

```csharp
public override string ConnectionString { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(((DBConnection)(workbook.DataConnections[1])).ConnectionString.IndexOf("$EmbeddedMashup(") == -1);
[Test]
        public void Property_ConnectionString()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava45985_1.xlsx");
            Workbook d = new Workbook(Constants.sourcePath + "CellsJava45985_2.xlsx");
            workbook.Combine(d);

            workbook.Save(Constants.destPath + "CellsJava45985.xlsx");

            workbook = new Workbook(Constants.destPath + "CellsJava45985.xlsx");
            Assert.AreEqual(2, workbook.DataMashup.PowerQueryFormulas.Count);
            Assert.IsTrue(((DBConnection)(workbook.DataConnections[1])).ConnectionString.IndexOf("$EmbeddedMashup(") == -1);
            //Console.WriteLine(workbook.Worksheets[0].Shapes[1].Text);
        }
```

### See Also

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


