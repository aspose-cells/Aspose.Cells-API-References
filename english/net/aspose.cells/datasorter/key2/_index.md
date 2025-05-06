---
title: DataSorter.Key2
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Represents second sorted column indexabsolute position column A is 0 B is 1 
type: docs
url: /net/aspose.cells/datasorter/key2/
---
## DataSorter.Key2 property

Represents second sorted column index(absolute position, column A is 0, B is 1, ...).

```csharp
public int Key2 { get; set; }
```

### Examples

```csharp
// Called: prev = cells[s1, sorter.Key2];
public static string Property_Key2(DataSorter sorter, Cells cells, CellArea range)
        {
            bool asending1 = sorter.Order1 == SortOrder.Ascending;
            bool asending2 = sorter.Order2 == SortOrder.Ascending;
            bool asending3 = sorter.Order3 == SortOrder.Ascending;
            Cell prev = cells[range.StartRow, sorter.Key1];
            string err = null;
            for (int r = range.StartRow + 1; r &lt;= range.EndRow; r++)
            {
                Cell cur1 = cells[r, sorter.Key1];
                int c = CheckSorted(prev, cur1, asending1, !sorter.CaseSensitive);
                if (c == 0)
                {
                    continue;
                }
                if (c &lt; 0)
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
                for (s1++; s1 &lt; r; s1++)
                {
                    Cell cur2 = cells[s1, sorter.Key2];
                    c = CheckSorted(prev, cur2, asending2, !sorter.CaseSensitive);
                    if (c == 0)
                    {
                        continue;
                    }
                    if (c &lt; 0)
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
                    for (s2++; s2 &lt; s1; s2++)
                    {
                        Cell cur3 = cells[s2, sorter.Key3];
                        c = CheckSorted(prev, cur3, asending3, !sorter.CaseSensitive);
                        if (c == 0)
                        {
                            continue;
                        }
                        if (c &lt; 0)
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
            sb.Append(&quot;\nCode to reproduce the bug:\nWorkbook wb = new Workbook(\&quot;SortErrorCheck.xlsx\&quot;);\nwb.DataSorter.Key1 = &quot;);
            sb.Append(sorter.Key1);
            sb.Append(&quot;;\nwb.DataSorter.Order1 = SortOrder.&quot;).Append(asending1 ? &quot;Ascending&quot; : &quot;Descending&quot;);
            sb.Append(&quot;;\nwb.DataSorter.Key2 = &quot;).Append(sorter.Key2);
            sb.Append(&quot;;\nwb.DataSorter.Order2 = SortOrder.&quot;).Append(asending2 ? &quot;Ascending&quot; : &quot;Descending&quot;);
            sb.Append(&quot;;\nwb.DataSorter.Key3 = &quot;).Append(sorter.Key3);
            sb.Append(&quot;;\nwb.DataSorter.Order3 = SortOrder.&quot;).Append(asending3 ? &quot;Ascending&quot; : &quot;Descending&quot;);
            sb.Append(&quot;;\nwb.DataSorter.CaseSensitive = &quot;).Append(sorter.CaseSensitive ? &quot;true&quot; : &quot;false&quot;);
            sb.Append(&quot;;\nCells sortedCells = wb.Worksheets[1].Cells;\nCellArea sortedRange = CellArea.CreateCellArea(&quot;);
            sb.Append(range.StartRow).Append(&apos;,&apos;).Append(range.StartColumn).Append(&apos;,&apos;);
            sb.Append(range.EndRow).Append(&apos;,&apos;).Append(range.EndColumn);
            sb.Append(&quot;);\nwb.DataSorter.Sort(sortedCells, sortedRange);\nConsole.WriteLine(DataSorterTest.Property_Key2(wb.DataSorter, sortedCells, sortedRange));\n&quot;);
            return sb.ToString();
        }
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


