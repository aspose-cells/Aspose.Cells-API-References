---
title: QueryTable.ConnectionId
second_title: Aspose.Cells for .NET API Reference
description: QueryTable property. Gets the connection id of the query table
type: docs
url: /net/aspose.cells/querytable/connectionid/
---
## QueryTable.ConnectionId property

Gets the connection id of the query table.

```csharp
public int ConnectionId { get; }
```

### Examples

```csharp
// Called: &amp;amp;&amp;amp; qt.ConnectionId &amp;gt;= 0)
public static void Property_ConnectionId(Workbook workbook, Aspose.Cells.ExternalConnections.ExternalConnection ec)
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

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


