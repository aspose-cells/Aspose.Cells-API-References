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
// Called: Assert.AreEqual("dd/MM/yyyy", style.InvariantCustom, "InvariantCustom");
        public void Style_Property_InvariantCustom()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();
            style.Number = 14;
            cell.PutValue(new DateTime(2019, 10, 12));
            cell.SetStyle(style);
#if !LINUX_TEST
            Assert.AreEqual("12.10.2019", cell.StringValue, "Formatted value");
            Assert.AreEqual("TT.MM.JJJJ", style.CultureCustom, "CultureCustom");
            Assert.AreEqual("dd/MM/yyyy", style.InvariantCustom, "InvariantCustom");
#else
            Assert.AreEqual("12.10.19", cell.StringValue, "Formatted value");
            Assert.AreEqual("TT.MM.JJ", style.CultureCustom, "CultureCustom");
            Assert.AreEqual("dd/MM/yy", style.InvariantCustom, "InvariantCustom");
#endif
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


