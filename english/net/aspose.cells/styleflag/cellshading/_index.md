---
title: StyleFlag.CellShading
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Cell shading setting will be applied
type: docs
url: /net/aspose.cells/styleflag/cellshading/
---
## StyleFlag.CellShading property

Cell shading setting will be applied.

```csharp
public bool CellShading { get; set; }
```

### Examples

```csharp
// Called: flag.CellShading = true;
[Test]
        public void Property_CellShading()
        {
            Workbook workbook = new Workbook();
            StyleFlag flag = new StyleFlag();
            flag.CellShading = true;
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("sdfsdfsdf");
            cells.ApplyRowStyle(0, style, flag);
            Assert.AreEqual(cells["A1"].GetStyle().Pattern, BackgroundType.Solid);
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


