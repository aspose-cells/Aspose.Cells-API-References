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
// Called: Assert.AreEqual(1000, vldt.Value2, &amp;quot;Validation.Value2&amp;quot;);
[Test]
        public void Property_Value2()
        {
            Workbook wb = new Workbook();
            ValidationCollection vldts = wb.Worksheets[0].Validations;
            Validation vldt = vldts[vldts.Add(CellArea.CreateCellArea(0, 0, 1, 1))];
            vldt.Operator = OperatorType.Between;
            vldt.Type = ValidationType.WholeNumber;
            vldt.Formula1 = &quot;-1000&quot;;
            vldt.Formula2 = &quot;1000&quot;;
            Assert.AreEqual(-1000, vldt.Value1, &quot;Validation.Value1&quot;);
            Assert.AreEqual(1000, vldt.Value2, &quot;Validation.Value2&quot;);
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


