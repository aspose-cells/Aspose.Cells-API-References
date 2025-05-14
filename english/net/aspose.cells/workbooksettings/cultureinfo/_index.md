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
public void WorkbookSettings_Property_CultureInfo()
{
    Workbook wb = new Workbook();
    wb.Settings.Region = CountryCode.France;
    Worksheet sheet = wb.Worksheets[0];

    string groupSep = wb.Settings.CultureInfo.NumberFormat.NumberGroupSeparator;
    //We do not know whether those white spaces should be changed or not, or how to change.
    //In my excel(my machine's region has been set as fr) they are changed to 32(' '),
    //but I am afraid it may be not true for fr OS.
    FormulaCaseUtil.StandaloneCalcTest(
        new string[]
        {
            "=TEXT(123456.78,\"# ###,00\u202f€\")", "=TEXT(123456.78,\"# ###,00 €\")",
            "=TEXT(123456.78,\"# ###,00\u202f €\")", "=TEXT(123456.78,\"# ###,00 \u202f€\")",
        },
        new object[]
        {
            "123" + groupSep +"456,78\u202f€", "123" + groupSep +"456,78 €",
            "123,46 €", "123,46\u202f€",
        },
        0, sheet, "");

    Style style = wb.CreateStyle();
    style.Custom = "#,##0.00_ ;-#,##0.00";
    Assert.AreEqual("#" + groupSep + "##0,00_ ;-#" + groupSep +"##0,00", style.CultureCustom, "CultureCustom from invariant");
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


