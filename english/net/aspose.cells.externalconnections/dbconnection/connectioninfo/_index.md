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
// Called: Assert.IsTrue(((DBConnection)(workbook.DataConnections[0])).ConnectionInfo.IndexOf(&amp;quot;$EmbeddedMashup(&amp;quot;) != -1);
[Test]
        public void Property_ConnectionInfo()
        {
            Workbook workbook = new Workbook();
            Workbook d = new Workbook(Constants.sourcePath + &quot;CellsJava45985_2.xlsx&quot;);
            workbook.Copy(d);

            workbook.Save(Constants.destPath + &quot;CellsJava45985_2.xlsx&quot;);

            workbook = new Workbook(Constants.destPath + &quot;CellsJava45985_2.xlsx&quot;);
            Assert.AreEqual(1, workbook.DataMashup.PowerQueryFormulas.Count);
            Assert.IsTrue(((DBConnection)(workbook.DataConnections[0])).ConnectionInfo.IndexOf(&quot;$EmbeddedMashup(&quot;) != -1);
            //Console.WriteLine(workbook.Worksheets[0].Shapes[1].Text);
        }
```

### See Also

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


