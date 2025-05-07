---
title: Cells.ApplyColumnStyle
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Applies formats for a whole column
type: docs
url: /net/aspose.cells/cells/applycolumnstyle/
---
## Cells.ApplyColumnStyle method

Applies formats for a whole column.

```csharp
public void ApplyColumnStyle(int column, Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | The column index. |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### Examples

```csharp
// Called: sheet.Cells.ApplyColumnStyle(0, style1, flag1);
[Test]
        public void Method_StyleFlag_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Style style1;
            StyleFlag flag1;

            style1 = wb.CreateStyle();
            style1.Number = 39;
            flag1 = new StyleFlag();
            flag1.All = true;

            //Apply style to the first column.
            sheet.Cells.ApplyColumnStyle(0, style1, flag1);
            Assert.AreEqual(wb.Worksheets[0].Cells["A1"].GetStyle().HorizontalAlignment, TextAlignmentType.General);

        }
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


