---
title: Validation.Areas
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Gets all CellArea which contain the data validation settings
type: docs
url: /net/aspose.cells/validation/areas/
---
## Validation.Areas property

Gets all [`CellArea`](../../cellarea/) which contain the data validation settings.

```csharp
public CellArea[] Areas { get; }
```

### Examples

```csharp
// Called: ca = (CellArea)dv.Areas[1];
	    public void Validation_Property_Areas()
	    {
            var d2 = new Validation_Property_Areas();
            Workbook workbook = d2.DoIt();
            Validation dv = workbook.Worksheets["Areas & rent"].Validations[0];
	        CellArea ca = (CellArea)dv.Areas[0];
            Assert.AreEqual(ca.StartRow, 46);
            ca = (CellArea)dv.Areas[1];
            Assert.AreEqual(ca.StartRow, 92);
            ca = (CellArea)dv.Areas[2];
            Assert.AreEqual(ca.StartRow, 138);
	    }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


