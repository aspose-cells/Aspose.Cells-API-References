---
title: Style.Pattern
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets the cell background pattern type
type: docs
url: /net/aspose.cells/style/pattern/
---
## Style.Pattern property

Gets or sets the cell background pattern type.

```csharp
public BackgroundType Pattern { get; set; }
```

### Examples

```csharp
// Called: testAreEqual(BackgroundType.Solid, cells[7, 4].GetStyle().Pattern, caseName);
private void Property_Pattern(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["sheetDest"];
            Cells cells = sheet.Cells;
            checkStyle(cells[3, 3].GetStyle());
            checkStyle(cells[4, 3].GetStyle());
            checkStyle(cells[5, 3].GetStyle());
            testequals(Color.Blue, cells[7, 3].GetStyle().ForegroundColor, caseName);
            testequals(Color.Blue, cells[7, 4].GetStyle().ForegroundColor, caseName);
            testAreEqual(BackgroundType.Solid, cells[7, 3].GetStyle().Pattern, caseName);
            testAreEqual(BackgroundType.Solid, cells[7, 4].GetStyle().Pattern, caseName);
            testequals(Color.Red, cells.Columns[4].GetStyle().ForegroundColor, caseName);
            testAreEqual(BackgroundType.Solid, cells.Columns[4].GetStyle().Pattern, caseName);
        }
```

### See Also

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


