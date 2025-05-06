---
title: Cells.Clear
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Clears all data of the worksheet
type: docs
url: /net/aspose.cells/cells/clear/
---
## Cells.Clear method

Clears all data of the worksheet.

```csharp
public void Clear()
```

### Examples

```csharp
// Called: cells.Clear();
[Test]
        public void Method_Clear()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            //ms excel does not make it as shared formula if part of the it may become #REF!
            //cells[0, 0].SetSharedFormula(&quot;=SUM(B1048573:B1048574)&quot;, 5, 1);
            //Assert.AreEqual(&quot;=SUM(#REF)&quot;, cells[4, 0].Formula);
            StringBuilder sb = new StringBuilder(32);
            sb.Append(&quot;=SUM(&quot;);
            for (int i = 0; i &lt; 32; i++)
            {
                sb.Length = 5;
                sb.Append((i &amp; 0x01) != 0 ? &quot;$A&quot; : &quot;A&quot;);
                if ((i &amp; 0x02) != 0)
                {
                    sb.Append(&apos;$&apos;);
                }
                if (i &lt; 16)
                {
                    sb.Append(i + 2);
                }
                else
                {
                    sb.Append(&quot;1048576&quot;);
                }
                sb.Append((i &amp; 0x04) != 0 ? &quot;:$B&quot; : &quot;:B&quot;);
                sb.Append((i &amp; 0x08) != 0 ? &quot;$1048576)&quot; : &quot;1048576)&quot;);
                cells[i, 5].SetSharedFormula(sb.ToString(), 1, 3);
            }
            cells.InsertRows(0, 1);
            cells.InsertRows(33, 1);
            for (int i = 0; i &lt; 16; i++)
            {
                for (int j = 0; j &lt; 3; j++)
                {
                    sb.Length = 5;
                    sb.Append((i &amp; 0x01) != 0 ? &quot;$A&quot; : ((char)(&apos;A&apos; + j)).ToString());
                    if ((i &amp; 0x02) != 0)
                    {
                        sb.Append(&apos;$&apos;);
                    }
                    sb.Append(i + 3);
                    sb.Append((i &amp; 0x04) != 0 ? &quot;:$B&quot; : &quot;:&quot; + (char)(&apos;B&apos; + j));
                    sb.Append((i &amp; 0x08) != 0 ? &quot;$1048576)&quot; : &quot;1048576)&quot;);
                    Assert.AreEqual(sb.ToString(), cells[i + 1, j + 5].Formula, i + &quot;-&quot; + j);
                    //Console.WriteLine(i + &quot;-&quot; + j + &quot;: Expected &quot; + sb.ToString() + &quot;, actual is &quot; + cells[i + 1, j + 5].Formula);
                }
            }
            for (int i = 16; i &lt; 32; i++)
            {
                for (int j = 0; j &lt; 3; j++)
                {
                    Assert.AreEqual(&quot;=SUM(#REF!)&quot;, cells[i + 1, j + 5].Formula, i + &quot;-&quot; + j);
                    //Console.WriteLine(i + &quot;-&quot; + j + &quot;: Expected =SUM(#REF!), actual is &quot; + cells[i + 1, j + 5].Formula);
                }
            }
            cells.Clear();
            for (int i = 0; i &lt; 16; i++)
            {
                sb.Length = 5;
                sb.Append((i &amp; 0x01) != 0 ? &quot;$B&quot; : &quot;B&quot;);
                sb.Append((i &amp; 0x02) != 0 ? &quot;$1&quot; : &quot;1&quot;);
                sb.Append((i &amp; 0x04) != 0 ? &quot;:$XFD&quot; : &quot;:XFD&quot;);
                sb.Append((i &amp; 0x08) != 0 ? &quot;$2)&quot; : &quot;2)&quot;);
                cells[5, i].SetSharedFormula(sb.ToString(), 3, 1);
            }
            cells.InsertColumns(0, 1);
            cells.InsertColumns(25, 1);
            for (int i = 0; i &lt; 16; i++)
            {
                for (int j = 0; j &lt; 3; j++)
                {
                    sb.Length = 5;
                    sb.Append((i &amp; 0x01) != 0 ? &quot;$C&quot; : &quot;C&quot;);
                    sb.Append((i &amp; 0x02) != 0 ? &quot;$1&quot; : (1 + j).ToString());
                    sb.Append((i &amp; 0x04) != 0 ? &quot;:$XFD&quot; : &quot;:XFD&quot;);
                    sb.Append((i &amp; 0x08) != 0 ? &quot;$2)&quot; : (2 + j) + &quot;)&quot;);
                    Assert.AreEqual(sb.ToString(), cells[j + 5, i + 1].Formula, j + &quot;-&quot; + i);
                    //Console.WriteLine(j + &quot;-&quot; + i + &quot;: Expected &quot; + sb.ToString() + &quot;, actual is &quot; + cells[j + 5, i + 1].Formula);
                }
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


