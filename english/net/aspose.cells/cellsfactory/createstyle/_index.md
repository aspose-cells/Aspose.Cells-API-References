---
title: CellsFactory.CreateStyle
second_title: Aspose.Cells for .NET API Reference
description: CellsFactory method. Creates a new style
type: docs
url: /net/aspose.cells/cellsfactory/createstyle/
---
## CellsFactory.CreateStyle method

Creates a new style.

```csharp
public Style CreateStyle()
```

### Return Value

Returns a style object.

### Examples

```csharp
// Called: var style = new CellsFactory().CreateStyle();
[Test]
        public void Method_CreateStyle()
        {
            var workbook = new Aspose.Cells.Workbook();
            var style = new CellsFactory().CreateStyle();
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thick, Color.Black);
            workbook.Worksheets[0].Cells["A1"].Value = "Hello";
            workbook.Worksheets[0].Cells["A1"].SetStyle(style);
            workbook.Save(Constants.destPath + "Cells55973.xlsx");
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + "Cells55973.xlsx", "xl/worksheets/sheet1.xml", new string[] { "thickBot=\"1\"" }, true));

        }
```

### See Also

* class [Style](../../style/)
* class [CellsFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


