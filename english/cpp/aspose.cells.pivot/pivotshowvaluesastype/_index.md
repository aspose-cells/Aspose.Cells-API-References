---
title: Aspose::Cells::Pivot::PivotShowValuesAsType enum
linktitle: PivotShowValuesAsType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotShowValuesAsType enum. Represents the calculation type for the "Show Values As" feature of pivot field values in C++.'
type: docs
weight: 5100
url: /cpp/aspose.cells.pivot/pivotshowvaluesastype/
---
## PivotShowValuesAsType enum


Represents the calculation type for the "Show Values As" feature of pivot field values.

```cpp
enum class PivotShowValuesAsType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Normal | 0 | <br>Represents raw value, no custom calculation. |
| DifferenceFrom | 1 | <br>Shows the value as the difference from a specified base item. |
| PercentageOf | 2 | <br>Shows the value as a percentage of a specified base item. |
| PercentageDifferenceFrom | 3 | <br>Shows the value as percentage difference from a specified base item. |
| RunningTotalIn | 4 | <br>Shows the value as a running total along the specified base field. |
| PercentageOfRow | 5 | <br>Shows the value as percentage of the row total. |
| PercentageOfColumn | 6 | <br>Shows the value as percentage of the column total. |
| PercentageOfTotal | 7 | <br>Shows the value as percentage of the grand total. |
| Index | 8 | <br>Index calculation: ([Cell](../../aspose.cells/cell/) Value × Grand Total of Grand Totals) / ([Row](../../aspose.cells/row/) Grand Total × [Column](../../aspose.cells/column/) Grand Total). |
| PercentageOfParentRowTotal | 9 | <br>Shows the value as percentage of its parent row item total. |
| PercentageOfParentColumnTotal | 10 | <br>Shows the value as percentage of its parent column item total. |
| PercentageOfParentTotal | 11 | <br>Shows the value as percentage of its parent item total in the specified base field. |
| PercentageOfRunningTotalIn | 12 | <br>Shows the value as percentage running total along the specified base field. |
| RankSmallestToLargest | 13 | <br>Ranks values from smallest to largest within the specified base field. |
| RankLargestToSmallest | 14 | <br>Ranks values from largest to smallest within the specified base field. |

## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
