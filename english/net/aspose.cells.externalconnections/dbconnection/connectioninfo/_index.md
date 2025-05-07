---
title: DBConnection.ConnectionInfo
second_title: Aspose.Cells for .NET API Reference
description: DBConnection property. The connection information string is used to make contact with an OLE DB or ODBC data source
type: docs
url: /net/aspose.cells.externalconnections/dbconnection/connectioninfo/
---
## DBConnection.ConnectionInfo property

The connection information string is used to make contact with an OLE DB or ODBC data source.

```csharp
[Obsolete("Use ExternalConnection.ConnectionString property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string ConnectionInfo { get; set; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use ExternalConnection.ConnectionString property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: Console.WriteLine(dbConn.ConnectionInfo);
[Test]
        public void Property_ConnectionInfo()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET47065.xlsx");
            ExternalConnectionCollection conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                DBConnection dbConn = conn as DBConnection;
                if (dbConn != null)
                {
                    Console.WriteLine(dbConn.ConnectionInfo);
                    Console.WriteLine(dbConn.PowerQueryFormula.FormulaDefinition);
                    Assert.IsFalse(dbConn.PowerQueryFormula.FormulaDefinition == null);
                }
            }
            workbook = new Workbook(Constants.sourcePath + "N47066.xlsm");
            conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                DBConnection dbConn = conn as DBConnection;
                if (dbConn != null)
                {
                    Console.WriteLine(dbConn.ConnectionInfo);
                    Console.WriteLine(dbConn.PowerQueryFormula.FormulaDefinition);
                    Assert.IsFalse(dbConn.PowerQueryFormula.FormulaDefinition == null);
                }
            }
        }
```

### See Also

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


