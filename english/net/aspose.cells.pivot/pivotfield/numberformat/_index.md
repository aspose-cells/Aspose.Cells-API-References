---
title: PivotField.NumberFormat
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the custom display format of numbers and dates
type: docs
url: /net/aspose.cells.pivot/pivotfield/numberformat/
---
## PivotField.NumberFormat property

Represents the custom display format of numbers and dates.

```csharp
public string NumberFormat { get; set; }
```

### Examples

```csharp
// Called: pivotField.NumberFormat = numberFormat;
private void PivotField_Property_NumberFormat(PivotTable pivotTable, string fieldName, string caption, string numberFormat,
            ConsolidationFunction consolidationFunction = ConsolidationFunction.Sum)
        {
            PivotField pivotField = pivotTable.DataFields[pivotTable.AddFieldToArea(PivotFieldType.Data, fieldName)];
            pivotField.DisplayName = caption;
            pivotField.Function = consolidationFunction;
            pivotField.NumberFormat = numberFormat;
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


