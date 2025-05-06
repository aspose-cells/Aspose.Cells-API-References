---
title: PivotTable.FormatAll
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Format all the cell in the pivottable area
type: docs
url: /net/aspose.cells.pivot/pivottable/formatall/
---
## PivotTable.FormatAll method

Format all the cell in the pivottable area

```csharp
public void FormatAll(Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | Style which is to format |

### Examples

```csharp
// Called: pt.FormatAll(st);
[Test]
        public void Method_Style_()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET44973_&quot;;

            Workbook wb = new Workbook(filePath + &quot;sample - 副本 (2).xlsx&quot;);
            Worksheet ws = wb.Worksheets[&quot;PivotTableSheet&quot;];

            PivotTable pt = ws.PivotTables[0];
            pt.RefreshDataOnOpeningFile = false;

            CellArea ca = pt.TableRange1;
            int idx1 = ca.ToString().IndexOf(&quot;(&quot;);
            int idx2 = ca.ToString().IndexOf(&quot;)&quot;);
            string address = ca.ToString().Substring(idx1 + 1, idx2 - idx1 - 1);

            Style st = wb.CreateStyle();
            st.Pattern = BackgroundType.Solid;
            st.ForegroundColor = Color.Red;
            st.BackgroundColor = Color.GreenYellow;


            ////Test 1:Colorizing the PivotTable.TableRange1
            //for (int r = ca.StartRow; r &lt;= ca.EndRow; r++)
            //{
            //    for (int c = ca.StartColumn; c &lt;= ca.EndColumn; c++)
            //    {
            //        //Debug.WriteLine(ws.Cells[r, c].Name);
            //        pt.Format(r, c, st);
            //    }
            //}


           // Test 2：This works fine
            pt.FormatAll(st);

            //Test 3: Apply via range also works fine
            //Range rng = ws.Cells.CreateRange(address);
            //StyleFlag flag = new StyleFlag();
            //flag.All = true;
            //rng.ApplyStyle(st, flag);

            wb.Save(CreateFolder(filePath) + &quot;out.xlsx&quot;);
        }
```

### See Also

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


