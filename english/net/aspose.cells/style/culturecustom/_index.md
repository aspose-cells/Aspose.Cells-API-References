---
title: Style.CultureCustom
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets and sets the culturedependent pattern string for number format. If no number format has been set for this object null will be returned. If number format is builtin the pattern string corresponding to the builtin number will be returned
type: docs
url: /net/aspose.cells/style/culturecustom/
---
## Style.CultureCustom property

Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned.

```csharp
public string CultureCustom { get; set; }
```

### Remarks

For builtin number format, both the pattern content(such as, one builtin date format is "m/d/y" for some locales, but for some other locales it becomes "d/m/y") and the format specifier(such as, some locales is using character other than 'y' to represent the year part for date formatting) are culture-dependent; For user specified custom format, only format specifiers are changed according to the culture, other parts of the formatting pattern will not be modified.

### Examples

```csharp
// Called: style.CultureCustom = cc;
[Test]
        public void Property_CultureCustom()
        {
            Workbook wb = new Workbook();
            wb.Settings.CultureInfo = new CultureInfo(&quot;hu-HU&quot;);
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();
            string c = &quot;yyyy-MM-dd hh:mm:ss ddd dddd MMM MMMM MMMMM&quot;;
            string cc = &quot;\u00e9\u00e9\u00e9\u00e9-hh-nn \u00f3\u00f3:pp:mm nnn nnnn hhh hhhh hhhhh&quot;; //éééé,óó
            style.Custom = c;
            Assert.AreEqual(cc, style.CultureCustom, &quot;CultureCustom from Custom&quot;);
            style.CultureCustom = cc;
            Assert.AreEqual(c, style.Custom, &quot;Custom from CultureCustom&quot;);
            cell.Formula = &quot;=TEXT(47512,\&quot;&quot; + cc + &quot;\&quot;)&quot;;
            cell.Calculate(new CalculationOptions());
            Assert.AreEqual(&quot;2030-01-29 00:00:00 K kedd jan. január j&quot;, cell.Value, &quot;Calcualted with culture formatting&quot;);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


