---
title: Workbook.GetMatchingColor
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Find best matching Color in current palette
type: docs
url: /net/aspose.cells/workbook/getmatchingcolor/
---
## Workbook.GetMatchingColor method

Find best matching Color in current palette.

```csharp
public Color GetMatchingColor(Color rawColor)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rawColor | Color | Raw color. |

### Return Value

Best matching color.

### Examples

```csharp
// Called: Color c = workbook.GetMatchingColor(Color.FromArgb(255, 123, 123, 123));
[Test]
        public void Method_Color_()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.CheckCompatibility = true;
            workbook.Save(Constants.destPath + "CellsNet40682.xls");
            workbook = new Workbook(Constants.destPath + "CellsNet40682.xls");
            Assert.AreEqual(workbook.Settings.CheckCompatibility, true);
            workbook.Settings.CheckCompatibility = false;
            workbook.Save(Constants.destPath + "CellsNet40682.xls");
            workbook = new Workbook(Constants.destPath + "CellsNet40682.xls");
            Assert.AreEqual(workbook.Settings.CheckCompatibility, false);
            Assert.IsTrue(workbook.IsColorInPalette(Color.Red));
            Assert.IsFalse(workbook.IsColorInPalette(Color.FromArgb(255,123,123,123)));
            Color c = workbook.GetMatchingColor(Color.FromArgb(255, 123, 123, 123));
            Assert.AreEqual(128, c.R);
            Color[] colors = new Color[12];
            for (int i = 0; i < colors.Length; i++)
            {
                colors[i] = Color.FromArgb(255, 128 + i, 128 + i, 128 + i);
            }
            workbook.CustomTheme("test", colors);
            c = workbook.GetThemeColor(ThemeColorType.FollowedHyperlink);
            Assert.AreEqual(139, c.R);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


