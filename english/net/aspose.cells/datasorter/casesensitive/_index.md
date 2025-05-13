---
title: DataSorter.CaseSensitive
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Gets and sets whether case sensitive when comparing string
type: docs
url: /net/aspose.cells/datasorter/casesensitive/
---
## DataSorter.CaseSensitive property

Gets and sets whether case sensitive when comparing string.

```csharp
public bool CaseSensitive { get; set; }
```

### Examples

```csharp
// Called: sorter.CaseSensitive = rp.NextDouble() > 0.5;
public void DataSorter_Property_CaseSensitive()
{ //CELLSNET-54905
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    Cells cells = sheet.Cells;
    Random rp = new Random();
    int rowCount = 10000;
    int nvUniqueCount = rowCount >> 2;
    Console.WriteLine("Generating test data...");
    for (int r = 0; r < rowCount; r++)
    {
        if (rp.NextDouble() < 0.01)
        {
            continue;
        }
        for (int c = 0; c < 3; c++)
        {
            int flag = (int)(rp.NextDouble() * 20);
            switch (flag)
            {
                case 0:
                {
                    continue;
                }
                case 1:
                {
                    flag = (int)(rp.NextDouble() * 20);
                    cells[r, c].PutValue((flag > 10 ? "v" : "V") + flag);
                    break;
                }
                case 2:
                {
                    cells[r, c].PutValue(rp.NextDouble() > 0.5);
                    break;
                }
                case 3:
                {
                    Cell cell = cells[r, c];
                    switch ((int)(rp.NextDouble() * 7))
                    {
                        case 0:
                        {
                            cell.PutValue("#DIV/0!");
                            break;
                        }
                        case 2:
                        {
                            cell.PutValue("#VALUE!");
                            break;
                        }
                        case 3:
                        {
                            cell.PutValue("#N/A");
                            break;
                        }
                        case 4:
                        {
                            cell.PutValue("#NAME?");
                            break;
                        }
                        case 5:
                        {
                            cell.PutValue("#NUM!");
                            break;
                        }
                        case 6:
                        {
                            cell.PutValue("#NULL!");
                            break;
                        }
                        case 7:
                        {
                            cell.PutValue("#REF!");
                            break;
                        }
                    }
                    break;
                }
                default:
                {
                    int iv = (int)(rp.NextDouble() * nvUniqueCount);
                    if (flag > 12)
                    {
                        cells[r, c].PutValue(iv);
                    }
                    else
                    {
                        cells[r, c].PutValue(iv + ((int)(rp.NextDouble() * 10.0)) / 10.0);
                    }
                    break;
                }
            }
        }
        cells[r, 3].PutValue(r);
    }
    wb.Worksheets.Add("Sheet2").Copy(sheet);
    DataSorter sorter = wb.DataSorter;
    int k = (int)(rp.NextDouble() * 3);
    sorter.Order1 = k > 1 ? SortOrder.Ascending : SortOrder.Descending;
    sorter.Key1 = k;
    sorter.Order2 = k > 2 ? SortOrder.Ascending : SortOrder.Descending;
    if (rp.NextDouble() > 0.5)
    {
        sorter.Key2 = 2 - k;
        sorter.Order3 = SortOrder.Ascending;
    }
    else
    {
        sorter.Key2 = (k + 1) % 3;
        sorter.Order3 = SortOrder.Descending;
    }
    sorter.Key3 = 3 - sorter.Key1 - sorter.Key2;
    sorter.CaseSensitive = rp.NextDouble() > 0.5;
    Console.WriteLine("Data generated. Sorting...");
    TimePerformance monitor = new TimePerformance(100);
    monitor.StartPerfTest();
    CellArea range = CellArea.CreateCellArea(0, 0, rowCount - 1, 3);
    sorter.Sort(cells, range);
    monitor.FinishPerfTest("Sorting large data set");
    Console.WriteLine("Finished");
    string err = VerifySorting(sorter, cells, range);
    if (err == null)
    {
        return;
    }
    Console.WriteLine(err);
    int pos = err.IndexOf("bug:\nWorkbook ") + 5;
    cells = wb.Worksheets[1].Cells;
    Style style = wb.CreateStyle();
    style.IsTextWrapped = true;
    Cell cc = cells[0, 4];
    cc.PutValue(err.Substring(0, pos));
    cc.SetStyle(style);
    cc = cells[1, 4];
    cc.PutValue(err.Substring(pos));
    cc.SetStyle(style);
    cells.SetColumnWidth(4, 100);
    wb.Save(Constants.destPath + "SortErrorCheck.xlsx");
    Assert.Fail("Incorrectly sorted result. Please check SortErrorCheck.xlsx in the destination path");
}
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


