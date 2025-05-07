---
title: WorkbookSettings.CheckCompatibility
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Indicates whether check compatibility with earlier versions when saving workbook
type: docs
url: /net/aspose.cells/workbooksettings/checkcompatibility/
---
## WorkbookSettings.CheckCompatibility property

Indicates whether check compatibility with earlier versions when saving workbook.

```csharp
public bool CheckCompatibility { get; set; }
```

### Remarks

The default value is true. Only for Excel97-2003 xls or xlt files.

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Settings.CheckCompatibility, false);
[Test]
        public void Property_CheckCompatibility()
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

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


