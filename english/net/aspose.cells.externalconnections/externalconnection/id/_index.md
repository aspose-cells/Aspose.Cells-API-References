---
title: ExternalConnection.Id
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Gets the id of the connection
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/id/
---
## ExternalConnection.Id property

Gets the id of the connection.

```csharp
public int Id { get; }
```

### Examples

```csharp
// Called: if (ec.Id == qt.ConnectionId
public static void Property_Id(Workbook workbook, Aspose.Cells.ExternalConnections.ExternalConnection ec)
        {
            for (int j = 0; j &lt; workbook.Worksheets.Count; j++)
            {
                Worksheet worksheet = workbook.Worksheets[j];
                for (int k = 0; k &lt; worksheet.QueryTables.Count; k++)
                {
                    Aspose.Cells.QueryTable qt = worksheet.QueryTables[k];
                    if (ec.Id == qt.ConnectionId
                        &amp;&amp; qt.ConnectionId &gt;= 0)
                    {
                        Console.WriteLine(&quot;querytable &quot; + qt.Name);
                        string n = qt.Name.Replace(&apos;+&apos;, &apos;_&apos;).Replace(&apos;=&apos;, &apos;_&apos;);
                        Name name = workbook.Worksheets.Names[&quot;&apos;&quot; + worksheet.Name + &quot;&apos;!&quot; + n];
                        if (name != null)
                        {
                            Aspose.Cells.Range range = name.GetRange();
                            if (range != null)
                            {
                                Console.WriteLine(&quot;refersto: &quot; + range.RefersTo);
                            }
                        }
                    }
                }
                for (int k = 0; k &lt; worksheet.ListObjects.Count; k++)
                {
                    ListObject table = worksheet.ListObjects[k];
                    if (table.DataSourceType == Aspose.Cells.Tables.TableDataSourceType.QueryTable)
                    {
                      
                        QueryTable qt = table.QueryTable;
                        if (ec.Id == qt.ConnectionId
                        &amp;&amp; qt.ConnectionId &gt;= 0)
                        {
                            if (k == 0)
                            {
                                Assert.AreEqual(table.StartRow, 0);
                            }
                            Console.WriteLine(&quot;querytable &quot; + qt.Name);
                            Console.WriteLine(&quot;Table &quot; + table.DisplayName);
                            Console.WriteLine(&quot;refersto: &quot; + worksheet.Name + &quot;!&quot; + CellsHelper.CellIndexToName(table.StartRow, table.StartColumn) + &quot;:&quot; + CellsHelper.CellIndexToName(table.EndRow, table.EndColumn));
                        }
                    }
                }
            }
        }
```

### See Also

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


