---
title: Enum LookInType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.LookInType enum. Represents look in type
type: docs
url: /net/aspose.cells/lookintype/
---
## LookInType enumeration

Represents look in type.

```csharp
public enum LookInType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Formulas | `0` | Finds the searched object from formula([`Formula`](../cell/formula/)) if the cell is formula, otherwise finds from cell's original value(same with OriginalValues). |
| Values | `1` | Finds object from cell's original value([`Value`](../cell/value/)) and formatted value([`StringValue`](../cell/stringvalue/)). |
| ValuesExcludeFormulaCell | `2` | Ignores cells that are formula. For those cells that are not formula, it is same with Values. |
| Comments | `3` | Finds object from cell's comment only. Ignores those cells that have no comment. |
| OnlyFormulas | `4` | Ignores cells that are not formula. For those cells that are formula, finds the searched object from formula([`Formula`](../cell/formula/)). |
| OriginalValues | `5` | Find object from cell's original value only. |
| FormattedValues | `6` | Find object from cell's formatted value([`StringValue`](../cell/stringvalue/)) only. |

### Examples

```csharp
// Called: { LookInType = LookInType.OnlyFormulas, LookAtType = LookAtType.Contains });
private void Cells_Type_LookInType(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells.Find("B1", null, new FindOptions()
            { LookInType = LookInType.OnlyFormulas, LookAtType = LookAtType.Contains });
            testAreEqual(1, cell.Row, caseName);
            testAreEqual(1, cell.Column, caseName);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


