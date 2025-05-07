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
// Called: && qt.ConnectionId >= 0)
public static void Property_ConnectionId(Workbook workbook, Aspose.Cells.ExternalConnections.ExternalConnection ec)
        {
            for (int j = 0; j < workbook.Worksheets.Count; j++)
            {
                Worksheet worksheet = workbook.Worksheets[j];
                for (int k = 0; k < worksheet.QueryTables.Count; k++)
                {
                    Aspose.Cells.QueryTable qt = worksheet.QueryTables[k];
                    if (ec.Id == qt.ConnectionId
                        && qt.ConnectionId >= 0)
                    {
                        Console.WriteLine("querytable " + qt.Name);
                        string n = qt.Name.Replace('+', '_').Replace('=', '_');
                        Name name = workbook.Worksheets.Names["'" + worksheet.Name + "'!" + n];
                        if (name != null)
                        {
                            Aspose.Cells.Range range = name.GetRange();
                            if (range != null)
                            {
                                Console.WriteLine("refersto: " + range.RefersTo);
                            }
                        }
                    }
                }
                for (int k = 0; k < worksheet.ListObjects.Count; k++)
                {
                    ListObject table = worksheet.ListObjects[k];
                    if (table.DataSourceType == Aspose.Cells.Tables.TableDataSourceType.QueryTable)
                    {
                      
                        QueryTable qt = table.QueryTable;
                        if (ec.Id == qt.ConnectionId
                        && qt.ConnectionId >= 0)
                        {
                            if (k == 0)
                            {
                                Assert.AreEqual(table.StartRow, 0);
                            }
                            Console.WriteLine("querytable " + qt.Name);
                            Console.WriteLine("Table " + table.DisplayName);
                            Console.WriteLine("refersto: " + worksheet.Name + "!" + CellsHelper.CellIndexToName(table.StartRow, table.StartColumn) + ":" + CellsHelper.CellIndexToName(table.EndRow, table.EndColumn));
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


