---
title: Style.Custom
second_title: Aspose.Cells for .NET API Reference
description: Style property. Represents the custom number format string of this style object. If the custom number format is not setFor example the number format is builtin  will be returned
type: docs
url: /net/aspose.cells/style/custom/
---
## Style.Custom property

Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned.

```csharp
public string Custom { get; set; }
```

### Remarks

The returned custom string is culture-independent.

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;令03.07.12&amp;quot;, cell.StringValue, style.Custom);
[Test]
        public void Property_Custom() //CELLSNET-47865,CELLSJAVA-43401
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.PutValue(44389);
            Style style = cell.GetStyle();
            style.Custom = &quot;ge.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;2021.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;geeee.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;2021.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;gey.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;202121.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;geyyy.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;20212021.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;ggeyyy.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;20212021.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;gggeyyy.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;20212021.07.12&quot;, cell.StringValue, style.Custom);

            style.Custom = &quot;[$-411]ge.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;R3.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;[$-411]geeee.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;R03.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;[$-411]gey.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;R303.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;[$-411]geyyy.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;R303.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;[$-411]gge.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;令3.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;[$-411]ggeeee.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;令03.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;[$-411]ggey.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;令303.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;[$-411]ggeyyy.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;令303.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;[$-411]ggge.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;令和3.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;[$-411]gggeeee.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;令和03.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;[$-411]gggey.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;令和303.07.12&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;[$-411]gggeyyy.mm.dd&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;令和303.07.12&quot;, cell.StringValue, style.Custom);

            style.Custom = &quot;[$-411]yge.mm.yyyyy&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;21R3.07.03&quot;, cell.StringValue, style.Custom);
            style.Custom = &quot;[$-411]yyyyyge.mm.yyyyy&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;2021R3.07.03&quot;, cell.StringValue, style.Custom);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


