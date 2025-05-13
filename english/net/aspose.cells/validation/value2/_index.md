---
title: Validation.Value2
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the second value associated with the data validation
type: docs
url: /net/aspose.cells/validation/value2/
---
## Validation.Value2 property

Represents the second value associated with the data validation.

```csharp
public object Value2 { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1000, vldt.Value2, "Validation.Value2");
public void Validation_Property_Value2()
{
    Workbook wb = new Workbook();
    ValidationCollection vldts = wb.Worksheets[0].Validations;
    Validation vldt = vldts[vldts.Add(CellArea.CreateCellArea(0, 0, 1, 1))];
    vldt.Operator = OperatorType.Between;
    vldt.Type = ValidationType.WholeNumber;
    vldt.Formula1 = "-1000";
    vldt.Formula2 = "1000";
    Assert.AreEqual(-1000, vldt.Value1, "Validation.Value1");
    Assert.AreEqual(1000, vldt.Value2, "Validation.Value2");
}
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


