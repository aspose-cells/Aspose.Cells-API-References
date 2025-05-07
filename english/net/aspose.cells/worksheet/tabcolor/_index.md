---
title: Worksheet.TabColor
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents worksheet tab color
type: docs
url: /net/aspose.cells/worksheet/tabcolor/
---
## Worksheet.TabColor property

Represents worksheet tab color.

```csharp
public Color TabColor { get; set; }
```

### Remarks

This feature is only supported in ExcelXP(Excel2002) and later versions. If you save file as Excel97 or Excel2000 format, it will be omitted.

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].TabColor.IsEmpty,true);
[Test]
        public void Property_TabColor()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava40330.xlsx");
            AssertHelper.AreEqual(workbook.Worksheets[0].TabColor, Color.Red);
            workbook.Worksheets[0].TabColor = Color.Empty;
            workbook.Save(Constants.destPath + "CellsJava40330.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsJava40330.xlsx");
            Assert.AreEqual(workbook.Worksheets[0].TabColor.IsEmpty,true);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


