---
title: WorkbookSettings.CultureInfo
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets or sets the system culture info
type: docs
url: /net/aspose.cells/workbooksettings/cultureinfo/
---
## WorkbookSettings.CultureInfo property

Gets or sets the system culture info.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Remarks

Returns null if culture info is not set and [`Region`](../region/) is not set.

### Examples

```csharp
// Called: string groupSep = wb.Settings.CultureInfo.NumberFormat.NumberGroupSeparator;
[Test]
        public void Property_CultureInfo()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.France;
            Worksheet sheet = wb.Worksheets[0];

            string groupSep = wb.Settings.CultureInfo.NumberFormat.NumberGroupSeparator;
            //We do not know whether those white spaces should be changed or not, or how to change.
            //In my excel(my machine&apos;s region has been set as fr) they are changed to 32(&apos; &apos;),
            //but I am afraid it may be not true for fr OS.
            FormulaCaseUtil.StandaloneCalcTest(
                new string[]
                {
                    &quot;=TEXT(123456.78,\&quot;# ###,00\u202f€\&quot;)&quot;, &quot;=TEXT(123456.78,\&quot;# ###,00 €\&quot;)&quot;,
                    &quot;=TEXT(123456.78,\&quot;# ###,00\u202f €\&quot;)&quot;, &quot;=TEXT(123456.78,\&quot;# ###,00 \u202f€\&quot;)&quot;,
                },
                new object[]
                {
                    &quot;123&quot; + groupSep +&quot;456,78\u202f€&quot;, &quot;123&quot; + groupSep +&quot;456,78 €&quot;,
                    &quot;123,46 €&quot;, &quot;123,46\u202f€&quot;,
                },
                0, sheet, &quot;&quot;);

            Style style = wb.CreateStyle();
            style.Custom = &quot;#,##0.00_ ;-#,##0.00&quot;;
            Assert.AreEqual(&quot;#&quot; + groupSep + &quot;##0,00_ ;-#&quot; + groupSep +&quot;##0,00&quot;, style.CultureCustom, &quot;CultureCustom from invariant&quot;);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


