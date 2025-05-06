---
title: Style.SetCustom
second_title: Aspose.Cells for .NET API Reference
description: Style method. Sets the Custom number format string of a cell
type: docs
url: /net/aspose.cells/style/setcustom/
---
## Style.SetCustom method

Sets the Custom number format string of a cell.

```csharp
public void SetCustom(string custom, bool builtinPreference)
```

| Parameter | Type | Description |
| --- | --- | --- |
| custom | String | Custom number format string, should be InvariantCulture pattern. |
| builtinPreference | Boolean | If given Custom number format string matches one of the built-in number formats corresponding to current regional settings, whether set the number format as built-in instead of Custom. |

### Examples

```csharp
// Called: style.SetCustom(p, true);
public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Style style = wb.CreateStyle();
            string p = &quot;_(\&quot;$\&quot;* #,##0.00_);_(\&quot;$\&quot;* (#,##0.00);_(\&quot;$\&quot;* \&quot;-\&quot;??_);_(@_)&quot;;
            style.SetCustom(p, true);
            Assert.AreEqual(44, style.Number, p);
            p = &quot;_($* #,##0.00_);_(\&quot;$\&quot;* (#,##0.00);_(\&quot;$\&quot;* \&quot;-\&quot;??_);_(@_)&quot;;
            style.SetCustom(p, true);
            Assert.AreEqual(44, style.Number, p);
            p = &quot;_($* #,##0.00_);_(\&quot;$\&quot;* (#,##0.00);_(\&quot;$\&quot;* -??_);_(@_)&quot;;
            style.SetCustom(p, true);
            Assert.AreEqual(44, style.Number, p);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


