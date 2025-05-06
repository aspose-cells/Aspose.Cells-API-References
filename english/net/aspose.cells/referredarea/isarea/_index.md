---
title: ReferredArea.IsArea
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. Indicates whether this is an area
type: docs
url: /net/aspose.cells/referredarea/isarea/
---
## ReferredArea.IsArea property

Indicates whether this is an area.

```csharp
public bool IsArea { get; }
```

### Remarks

If this is not an area, only StartRow and StartColumn effect.

### Examples

```csharp
// Called: if (ra.IsArea != (i == 0))
[Test]
        public void Property_IsArea()
        {
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells[3, 3].PutValue(&quot;v03&quot;);
            Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add(&quot;testname&quot;)];
            n.RefersTo = &quot;=&apos;C:\\[extlink1.xlsx]Sheet1&apos;!$A$1:$B$2,&apos;C:\\[extlink2.xlsx]Sheet2&apos;!$C$3,Sheet1!$D$4,&apos;C:\\[extlink1.xlsx]Sheet1&apos;!E5&quot;;
            Aspose.Cells.Range[] rs = n.GetRanges(true);
            if (rs == null)
            {
                Assert.Fail(&quot;GetRanges should not return null&quot;);
            }
            else if (rs.Length != 1)
            {
                Assert.Fail(&quot;GetRanges gives incorrect count of ranges: &quot; + rs.Length);
            }
            else
            {
                if (rs[0].RowCount &gt; 1 || rs[0].ColumnCount &gt; 1)
                {
                    Assert.Fail(&quot;Got range should be single&quot;);
                }
                if (rs[0].FirstRow != 3 || rs[0].FirstColumn != 3)
                {
                    Assert.Fail(&quot;Incorrect address for returned Range: &quot;
                        + CellsHelper.CellIndexToName(rs[0].FirstRow, rs[0].FirstColumn));
                }
            }
            ReferredArea[] ras = n.GetReferredAreas(true);
            if (ras == null)
            {
                Assert.Fail(&quot;GetReferredAreas should not return null&quot;);
            }
            if (ras.Length != 4)
            {
                Assert.Fail(&quot;GetReferredAreas gives incorrect count of areas: &quot; + ras.Length);
            }
            for (int i = 0; i &lt; ras.Length; i++)
            {
                ReferredArea ra = ras[i];
                if (i == 2)
                {
                    if (ra.IsExternalLink)
                    {
                        Assert.Fail(&quot;Areas[2] should not be ExternalLink&quot;);
                    }
                }
                else
                {
                    if (!ra.IsExternalLink)
                    {
                        Assert.Fail(i + &quot;: should be ExternalLink&quot;);
                    }
                    if (&quot;C:\\extlink&quot; + (i == 1 ? 2 : 1) + &quot;.xlsx&quot; != ra.ExternalFileName)
                    {
                        Assert.Fail(i + &quot;: Incorrect value of ExternalFileName[&quot; + ra.ExternalFileName + &quot;]&quot;);
                    }
                }
                if(&quot;Sheet&quot; + (i==1 ? 2 : 1) != ra.SheetName)
                {
                    Assert.Fail(i + &quot;: Incorrect value of SheetName[&quot; + ra.SheetName + &quot;]&quot;);
                }
                if (ra.IsArea != (i == 0))
                {
                    Assert.Fail(i + &quot;: Incorrect value of IsArea[&quot; + ra.IsArea + &quot;]&quot;);
                }
                if (i == 0)
                {
                    if (ra.StartRow != 0 || ra.StartColumn != 0 || ra.EndRow != 1 || ra.EndColumn != 1)
                    {
                        Assert.Fail(i + &quot;: Incorrect area[&quot; + CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)
                            + &quot;:&quot; + CellsHelper.CellIndexToName(ra.EndRow, ra.EndColumn) + &quot;]&quot;);
                    }
                }
                else
                {
                    if (ra.StartRow != i + 1 || ra.StartColumn != i + 1)
                    {
                        Assert.Fail(i + &quot;: Incorrect address[&quot; + CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn) + &quot;]&quot;);
                    }
                }
            }
            Workbook wb1 = new Workbook();
            wb1.FileName = &quot;C:\\extlink1.xlsx&quot;;
            Cells cells = wb1.Worksheets[0].Cells;
            for (int i = 0; i &lt; 5; i++)
            {
                cells[i, i].PutValue(&quot;v1&quot; + i);
            }
            wb.UpdateLinkedDataSource(new Workbook[]{wb1});
            Assert.AreEqual(&quot;v10&quot;, ras[0].GetValue(0, 0));
            Assert.AreEqual(&quot;v11&quot;, ras[0].GetValue(1, 1));
            Assert.AreEqual(&quot;#REF!&quot;, ras[1].GetValue(0, 0));
            Assert.AreEqual(&quot;v03&quot;, ras[2].GetValue(0, 0));
            Assert.AreEqual(&quot;v14&quot;, ras[3].GetValue(0, 0));
        }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


