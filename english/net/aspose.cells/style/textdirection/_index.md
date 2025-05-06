---
title: Style.TextDirection
second_title: Aspose.Cells for .NET API Reference
description: Style property. Represents text reading order
type: docs
url: /net/aspose.cells/style/textdirection/
---
## Style.TextDirection property

Represents text reading order.

```csharp
public TextDirectionType TextDirection { get; set; }
```

### Examples

```csharp
// Called: testAreEqual(TextDirectionType.Context, cells[0, 0].GetStyle().TextDirection, caseName);
private void Property_TextDirection(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            testAreEqual(TextDirectionType.Context, cells[0, 0].GetStyle().TextDirection, caseName);
        }
```

### See Also

* enum [TextDirectionType](../../textdirectiontype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


