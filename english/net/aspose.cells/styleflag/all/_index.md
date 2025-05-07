---
title: StyleFlag.All
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. All properties will be applied
type: docs
url: /net/aspose.cells/styleflag/all/
---
## StyleFlag.All property

All properties will be applied.

```csharp
public bool All { get; set; }
```

### Examples

```csharp
// Called: flag.All = true;
[Test]
        public void Property_All()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "ApplyNamedStyle_126777.xls");
            Style style = workbook.GetNamedStyle("test");
            StyleFlag flag = new StyleFlag();
            flag.All = true;
            workbook.Worksheets[0].Cells.ApplyRowStyle(4, style, flag);

            workbook.Save(Constants.destPath + "ApplyNamedStyle_126777.xls");
            workbook = new Workbook(Constants.destPath + "ApplyNamedStyle_126777.xls");
            Cell cell = workbook.Worksheets[0].Cells[4, 0];
            Assert.AreEqual(cell.GetStyle().Font.Color.ToArgb() & 0xFFFFFF,
                System.Drawing.Color.Red.ToArgb() & 0xFFFFFF);
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


