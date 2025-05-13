---
title: Style.Custom
second_title: Aspose.Cells for .NET API Reference
description: Style property. Represents the custom number format string of this style object. If the custom number format is not setFor example the number format is builtin  will be returned
type: docs
url: /net/aspose.cells/style/custom/
---
## Style.Custom property

Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned.

```csharp
public string Custom { get; set; }
```

### Remarks

The returned custom string is culture-independent.

### Examples

```csharp
// Called: style.Custom = "d-mmm-yy";
public void Style_Property_Custom()
{
  Workbook workbook = new Workbook();
  Cells cells = workbook.Worksheets[0].Cells;
  Style style = workbook.CreateStyle();
  style.Custom = "d-mmm-yy";
  cells[0, 0].PutValue(1999);
  cells[0, 0].SetStyle(style);
  cells[0, 1].Formula = "=CELL(\"format\", A1)";
  Console.WriteLine("=CELL(\"format\", A1)");
  workbook.CalculateFormula();
  Assert.AreEqual("D1", cells[0, 1].StringValue);
}
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


