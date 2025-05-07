---
title: Style.IndentLevel
second_title: Aspose.Cells for .NET API Reference
description: Style property. Represents the indent level for the cell or range. Can only be an integer from 0 to 250
type: docs
url: /net/aspose.cells/style/indentlevel/
---
## Style.IndentLevel property

Represents the indent level for the cell or range. Can only be an integer from 0 to 250.

```csharp
public int IndentLevel { get; set; }
```

### Remarks

If text horizontal alignment type is set to value other than left or right, indent level will be reset to zero.

### Examples

```csharp
// Called: testAreEqual(4, cells[4, 0].GetStyle().IndentLevel, caseName);
private void Property_IndentLevel(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            testAreEqual(0, cells[0, 0].GetStyle().IndentLevel, caseName);
            testAreEqual(1, cells[1, 0].GetStyle().IndentLevel, caseName);
            testAreEqual(2, cells[2, 0].GetStyle().IndentLevel, caseName);
            testAreEqual(3, cells[3, 0].GetStyle().IndentLevel, caseName);
            testAreEqual(4, cells[4, 0].GetStyle().IndentLevel, caseName);
            testAreEqual(5, cells[5, 0].GetStyle().IndentLevel, caseName);
            testAreEqual(6, cells[6, 0].GetStyle().IndentLevel, caseName);
            testAreEqual(7, cells[7, 0].GetStyle().IndentLevel, caseName);
            testAreEqual(8, cells[8, 0].GetStyle().IndentLevel, caseName);
            testAreEqual(9, cells[9, 0].GetStyle().IndentLevel, caseName);
            testAreEqual(10, cells[10, 0].GetStyle().IndentLevel, caseName);
            testAreEqual(11, cells[11, 0].GetStyle().IndentLevel, caseName);
            testAreEqual(12, cells[12, 0].GetStyle().IndentLevel, caseName);
            testAreEqual(13, cells[13, 0].GetStyle().IndentLevel, caseName);
            testAreEqual(14, cells[14, 0].GetStyle().IndentLevel, caseName);
            testAreEqual(15, cells[15, 0].GetStyle().IndentLevel, caseName);

            for (int i = 1; i < 16; i++)
            {
                testAreEqual(TextAlignmentType.Left, cells[i, 0].GetStyle().HorizontalAlignment, caseName);
            }
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


