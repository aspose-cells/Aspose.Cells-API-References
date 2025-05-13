---
title: DataSorter.Order3
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Represents sort order of the third key
type: docs
url: /net/aspose.cells/datasorter/order3/
---
## DataSorter.Order3 property

Represents sort order of the third key.

```csharp
public SortOrder Order3 { get; set; }
```

### Examples

```csharp
// Called: bool asending3 = sorter.Order3 == SortOrder.Ascending;
public static string DataSorter_Property_Order3(DataSorter sorter, Cells cells, CellArea range)
        {
            bool asending1 = sorter.Order1 == SortOrder.Ascending;
            bool asending2 = sorter.Order2 == SortOrder.Ascending;
            bool asending3 = sorter.Order3 == SortOrder.Ascending;
            Cell prev = cells[range.StartRow, sorter.Key1];
            string err = null;
            for (int r = range.StartRow + 1; r <= range.EndRow; r++)
            {
                Cell cur1 = cells[r, sorter.Key1];
                int c = CheckSorted(prev, cur1, asending1, !sorter.CaseSensitive);
                if (c == 0)
                {
                    continue;
                }
                if (c < 0)
                {
                    err = BuildErrorSorting(prev, cur1);
                    break;
                }
                if (prev.Row + 1 == r)
                {
                    prev = cur1;
                    continue;
                }
                int s1 = prev.Row;
                prev = cells[s1, sorter.Key2];
                for (s1++; s1 < r; s1++)
                {
                    Cell cur2 = cells[s1, sorter.Key2];
                    c = CheckSorted(prev, cur2, asending2, !sorter.CaseSensitive);
                    if (c == 0)
                    {
                        continue;
                    }
                    if (c < 0)
                    {
                        err = BuildErrorSorting(prev, cur2);
                        break;
                    }
                    if (prev.Row + 1 == s1)
                    {
                        prev = cur2;
                        continue;
                    }
                    int s2 = prev.Row;
                    prev = cells[s2, sorter.Key3];
                    for (s2++; s2 < s1; s2++)
                    {
                        Cell cur3 = cells[s2, sorter.Key3];
                        c = CheckSorted(prev, cur3, asending3, !sorter.CaseSensitive);
                        if (c == 0)
                        {
                            continue;
                        }
                        if (c < 0)
                        {
                            err = BuildErrorSorting(prev, cur3);
                            break;
                        }
                        prev = cur3;
                    }
                    if (err != null)
                    {
                        break;
                    }
                    prev = cur2;
                }
                if (err != null)
                {
                    break;
                }
                prev = cur1;
            }
            if (err == null)
            {
                return null;
            }
            StringBuilder sb = new StringBuilder();
            sb.Append(err);
            sb.Append("\nCode to reproduce the bug:\nWorkbook wb = new Workbook(\"SortErrorCheck.xlsx\");\nwb.DataSorter.Key1 = ");
            sb.Append(sorter.Key1);
            sb.Append(";\nwb.DataSorter.Order1 = SortOrder.").Append(asending1 ? "Ascending" : "Descending");
            sb.Append(";\nwb.DataSorter.Key2 = ").Append(sorter.Key2);
            sb.Append(";\nwb.DataSorter.Order2 = SortOrder.").Append(asending2 ? "Ascending" : "Descending");
            sb.Append(";\nwb.DataSorter.Key3 = ").Append(sorter.Key3);
            sb.Append(";\nwb.DataSorter.Order3 = SortOrder.").Append(asending3 ? "Ascending" : "Descending");
            sb.Append(";\nwb.DataSorter.CaseSensitive = ").Append(sorter.CaseSensitive ? "true" : "false");
            sb.Append(";\nCells sortedCells = wb.Worksheets[1].Cells;\nCellArea sortedRange = CellArea.CreateCellArea(");
            sb.Append(range.StartRow).Append(',').Append(range.StartColumn).Append(',');
            sb.Append(range.EndRow).Append(',').Append(range.EndColumn);
            sb.Append(");\nwb.DataSorter.Sort(sortedCells, sortedRange);\nConsole.WriteLine(DataSorterTest.DataSorter_Property_Order3(wb.DataSorter, sortedCells, sortedRange));\n");
            return sb.ToString();
        }
```

### See Also

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


