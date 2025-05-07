---
title: Style.SetPatternColor
second_title: Aspose.Cells for .NET API Reference
description: Style method. Sets the background color
type: docs
url: /net/aspose.cells/style/setpatterncolor/
---
## Style.SetPatternColor method

Sets the background color.

```csharp
public void SetPatternColor(BackgroundType pattern, Color color1, Color color2)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pattern | BackgroundType | The pattern. |
| color1 | Color | The foreground color. |
| color2 | Color | The background color. Only works when pattern is not BackgroundType.None and BackgroundType.Solid. |

### Examples

```csharp
// Called: style.SetPatternColor(BackgroundType.Solid, Color.Red, Color.Red);
[Test]
	    public void Method_Color_()
	    {
            Workbook workbook = new Workbook();
	        Cell cell = workbook.Worksheets[0].Cells["A1"];
	        Style style = cell.GetStyle();
	        style.SetPatternColor(BackgroundType.Solid, Color.Red, Color.Red);
            Assert.AreEqual(BackgroundType.Solid, style.Pattern, "Pattern");
            AssertHelper.AreEqual(Color.Red, style.ForegroundColor, "ForegroundColor");
            Util.ReSave(workbook, SaveFormat.Xlsx);
	    }
```

### See Also

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


