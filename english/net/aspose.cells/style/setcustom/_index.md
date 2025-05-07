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
// Called: style.SetCustom("$#,##0_);($#,##0)", true);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Style style = wb.CreateStyle();
            style.SetCustom("$#,##0_);($#,##0)", true);
            Assert.AreEqual(5, style.Number, "Corresponding builtin number");
            Assert.AreEqual("", style.Custom, "Style.Custom");
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


