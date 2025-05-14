---
title: QueryTable.Name
second_title: Aspose.Cells for .NET API Reference
description: QueryTable property. Gets the name of querytable
type: docs
url: /net/aspose.cells/querytable/name/
---
## QueryTable.Name property

Gets the name of querytable.

```csharp
public string Name { get; }
```

### Examples

```csharp
// Called: Console.WriteLine("querytable " + qt.Name);
public static void QueryTable_Property_Name(Workbook workbook, Aspose.Cells.ExternalConnections.ExternalConnection ec)
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


