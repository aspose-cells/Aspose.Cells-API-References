---
title: Cells.SetRowHeightPixel
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Sets row height in unit of pixels
type: docs
url: /net/aspose.cells/cells/setrowheightpixel/
---
## Cells.SetRowHeightPixel method

Sets row height in unit of pixels.

```csharp
public void SetRowHeightPixel(int row, int pixels)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| pixels | Int32 | Number of pixels. |

### Examples

```csharp
// Called: cells.SetRowHeightPixel(i, 10 + i % 10);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 500000; i++)
            {
                if (i % 10 &gt; 3)
                {
                    cells.SetRowHeightPixel(i, 10 + i % 10);
                }
            }
            int dh = cells.StandardHeightPixels;
            TimePerformance monitor = new TimePerformance(180);
            monitor.StartPerfTest();
            for (int i = 0; i &lt; 100000; i++)
            {
                if (i % 10000 == 0)
                {
                    Console.WriteLine(&quot;Searching row &quot; + i);
                }
                int h0 = cells.GetRowHeightPixel(i);
                int h1 = cells.GetRowHeightPixel(i + 100000);
                int h2 = cells.GetRowHeightPixel(i + 200000);
                int h3 = cells.GetRowHeightPixel(i + 300000);
                int h4 = cells.GetRowHeightPixel(i + 400000);
                if (i % 10000 &lt; 10)
                {
                    Assert.AreEqual(i % 10 &gt; 3 ? 10 + i % 10 : dh, h0, i + &quot;.HeightPixel&quot;);
                    if (h0 != h1 || h0 != h2 || h0 != h3 || h0 != h4)
                    {
                        Assert.Fail(&quot;Wrong height value: &quot; + h0 + &quot;,&quot; + h1 + &quot;,&quot; + h2 + &quot;,&quot; + h3 + &quot;,&quot; + h4);
                    }
                }
            }
            monitor.FinishPerfTest();
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


