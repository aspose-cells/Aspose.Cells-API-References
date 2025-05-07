---
title: FontConfigs.SetFontFolder
second_title: Aspose.Cells for .NET API Reference
description: FontConfigs method. Sets the fonts folder
type: docs
url: /net/aspose.cells/fontconfigs/setfontfolder/
---
## FontConfigs.SetFontFolder method

Sets the fonts folder

```csharp
public static void SetFontFolder(string fontFolder, bool recursive)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fontFolder | String | The folder that contains TrueType fonts. |
| recursive | Boolean | Determines whether or not to scan subfolders. |

### Examples

```csharp
// Called: FontConfigs.SetFontFolder(dir + "fonts", true);
[Test]
        public void Method_Boolean_()
        {
            string dir = Constants.sourcePath + "/CELLSNET-44002/";
            FontConfigs.SetFontFolder(dir + "fonts", true);

            Workbook wb = new Workbook(dir + "CELLSNET-44002.xlsx");
            Worksheet sheet = wb.Worksheets[0];
            sheet.AutoFitRows(true);
            Cells cells = sheet.Cells;

            Assert.AreEqual(28, cells.GetRowHeightPixel(0));
            Assert.AreEqual(24, cells.GetRowHeightPixel(9));
        }
```

### See Also

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


