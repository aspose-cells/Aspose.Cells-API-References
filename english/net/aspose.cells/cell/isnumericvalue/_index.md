---
title: Cell.IsNumericValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates whether the value of this cell is numericint double and datetime
type: docs
url: /net/aspose.cells/cell/isnumericvalue/
---
## Cell.IsNumericValue property

Indicates whether the value of this cell is numeric(int, double and datetime)

```csharp
public bool IsNumericValue { get; }
```

### Remarks

Also applies to formula cell to check the calculated result

### Examples

```csharp
// Called: if (cell2.IsNumericValue)
private static bool Property_IsNumericValue(Cell cell1, Cell cell2, double delta)
        {
            if (cell1.IsNumericValue)
            {
                if (cell2.IsNumericValue)
                {
                    return IsEqual(cell1.DoubleValue, cell2.DoubleValue, delta);
                }
                return false;
            }
            else if (cell2.IsNumericValue)
            {
                return false;
            }
            CellValueType vt = cell1.Type;
            if (vt != cell2.Type)
            {
                return vt == CellValueType.IsNull && cell2.Type == CellValueType.IsString && cell2.StringValue == ""
                    || vt == CellValueType.IsString && cell2.Type == CellValueType.IsNull && cell1.StringValue == "";
            }
            if (vt == CellValueType.IsNull)
            {
                return true;
            }
            if (vt == CellValueType.IsString)
            {
                return cell1.StringValue.Replace("\r\n", "\n") == cell2.StringValue.Replace("\r\n", "\n");
            }
            return cell1.Value.Equals(cell2.Value);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


