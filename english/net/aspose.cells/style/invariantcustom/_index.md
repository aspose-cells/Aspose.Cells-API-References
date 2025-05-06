---
title: Style.InvariantCustom
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets the cultureindependent pattern string for number format. If no number format has been set for this object null will be returned. If number format is builtin the pattern string corresponding to the builtin number will be returned
type: docs
url: /net/aspose.cells/style/invariantcustom/
---
## Style.InvariantCustom property

Gets the culture-independent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned.

```csharp
public string InvariantCustom { get; }
```

### Remarks

For builtin number formats, the returned pattern content is still culture-dependent, such as, for some locales it returns "m/d/y" and for some other locales it returns "d/m/y". The difference from [`CultureCustom`](../culturecustom/) is(that is also what culture-independent means): the format specifiers and separators are kept as standard, such as '/' will always be used as datetime separator and "y" will always be used as the "year" part no matter what other special character is used for the specific locale.

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;dd/MM/yyyy&amp;quot;, style.InvariantCustom, &amp;quot;InvariantCustom&amp;quot;);
[Test]
        public void Property_InvariantCustom()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();
            style.Number = 14;
            cell.PutValue(new DateTime(2019, 10, 12));
            cell.SetStyle(style);
#if !LINUX_TEST
            Assert.AreEqual(&quot;12.10.2019&quot;, cell.StringValue, &quot;Formatted value&quot;);
            Assert.AreEqual(&quot;TT.MM.JJJJ&quot;, style.CultureCustom, &quot;CultureCustom&quot;);
            Assert.AreEqual(&quot;dd/MM/yyyy&quot;, style.InvariantCustom, &quot;InvariantCustom&quot;);
#else
            Assert.AreEqual(&quot;12.10.19&quot;, cell.StringValue, &quot;Formatted value&quot;);
            Assert.AreEqual(&quot;TT.MM.JJ&quot;, style.CultureCustom, &quot;CultureCustom&quot;);
            Assert.AreEqual(&quot;dd/MM/yy&quot;, style.InvariantCustom, &quot;InvariantCustom&quot;);
#endif
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


