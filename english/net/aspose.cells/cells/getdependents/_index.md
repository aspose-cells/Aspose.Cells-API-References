---
title: Cells.GetDependents
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Get all cells which refer to the specific cell
type: docs
url: /net/aspose.cells/cells/getdependents/
---
## Cells.GetDependents method

Get all cells which refer to the specific cell.

```csharp
public Cell[] GetDependents(bool isAll, int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isAll | Boolean | Indicates whether check other worksheets |
| row | Int32 | The row index. |
| column | Int32 | The column index. |

### Examples

```csharp
// Called: Cell[] res = cells.GetDependents(false, i, 1);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            wb.Worksheets.Names[wb.Worksheets.Names.Add(&quot;MyTestName&quot;)].RefersTo = &quot;=Sheet1!B1&quot;;
            for (int i = 0; i &lt; 5; i++)
            {
                cells[i, 0].Formula = &quot;=MyTestName&quot;;
            }
            for (int i = 0; i &lt; 5; i++)
            {
                Cell[] res = cells.GetDependents(false, i, 1);
                if (res == null || res.Length &lt; 1)
                {
                    Assert.Fail(&quot;B&quot; + (i + 1) + &quot;&apos;s dependents should be A&quot; + (i + 1) + &quot;, but got null&quot;);
                }
                if (res.Length &gt; 1)
                {
                    StringBuilder sb = new StringBuilder();
                    sb.Append(&apos;B&apos;);
                    sb.Append(i + 1);
                    sb.Append(&quot;&apos;s dependents should be only A&quot;);
                    sb.Append(i + 1);
                    sb.Append(&quot;, but got &quot;);
                    sb.Append(res.Length);
                    sb.Append(&quot; cells: [&quot;);
                    foreach (Cell item in res)
                    {
                        sb.Append(item.Name);
                        sb.Append(&apos;,&apos;);
                    }
                    sb[sb.Length - 1] = &apos;]&apos;;
                    Assert.Fail(sb.ToString());
                }
                Cell c = res[0];
                if (c.Column != 0 || c.Row != i)
                {
                    Assert.Fail(&quot;B&quot; + (i + 1) + &quot;&apos;s dependents should be A&quot; + (i + 1) + &quot;, but got &quot; + c.Name);
                }
            }
        }
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


