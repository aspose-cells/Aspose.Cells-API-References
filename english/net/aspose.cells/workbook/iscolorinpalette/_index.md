---
title: Workbook.IsColorInPalette
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Checks if a color is in the palette for the spreadsheet
type: docs
url: /net/aspose.cells/workbook/iscolorinpalette/
---
## Workbook.IsColorInPalette method

Checks if a color is in the palette for the spreadsheet.

```csharp
public bool IsColorInPalette(Color color)
```

| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | Color structure. |

### Return Value

Returns true if this color is in the palette. Otherwise, returns false

### Examples

```csharp
// Called: Assert.IsFalse(workbook.IsColorInPalette(Color.FromArgb(255,123,123,123)));
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


