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
// Called: { LookInType = LookInType.OnlyFormulas, LookAtType = LookAtType.EntireContent });
private void Type_LookInType(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells.Find(&quot;=SUM(Sheet1!A1:B1)&quot;, null, new FindOptions()
            { LookInType = LookInType.OnlyFormulas, LookAtType = LookAtType.EntireContent });
            testAreEqual(null, cell, caseName);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


