---
title: WorkbookSettings.GetThemeFont
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings method. Gets the default theme font name
type: docs
url: /net/aspose.cells/workbooksettings/getthemefont/
---
## WorkbookSettings.GetThemeFont method

Gets the default theme font name.

```csharp
public string GetThemeFont(FontSchemeType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | FontSchemeType | The scheme type of the font. |

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;Cambria&amp;quot;, wb.Settings.GetThemeFont(FontSchemeType.Major));
[Test]
        public void Method_FontSchemeType_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-49334.xls&quot;);

            Assert.AreEqual(&quot;Calibri&quot;, wb.Settings.GetThemeFont(FontSchemeType.Minor));
            Assert.AreEqual(&quot;Cambria&quot;, wb.Settings.GetThemeFont(FontSchemeType.Major));
        }
```

### See Also

* enum [FontSchemeType](../../fontschemetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


