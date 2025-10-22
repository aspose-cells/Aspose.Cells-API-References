##LookInType
Represents look in type.
## LookInType enumeration
Represents look in type.
### Values
| Name | Value | Description |
| --- | --- | --- |
| Formulas | `0` | Finds the searched object from formula([Cell.Formula](../cell.formula/)) if the cell is formula, otherwise finds from cell's original value(same with [OriginalValues](../originalvalues/)). |
| Values | `1` | Finds object from cell's original value([Cell.Value](../cell.value/)) and formatted value([Cell.StringValue](../cell.stringvalue/)). |
| ValuesExcludeFormulaCell | `2` | Ignores cells that are formula. For those cells that are not formula, it is same with [Values](../values/). |
| Comments | `3` | Finds object from cell's comment only. Ignores those cells that have no comment. |
| OnlyFormulas | `4` | Ignores cells that are not formula. For those cells that are formula, finds the searched object from formula([Cell.Formula](../cell.formula/)). |
| OriginalValues | `5` | Find object from cell's original value only. |
| FormattedValues | `6` | Find object from cell's formatted value([Cell.StringValue](../cell.stringvalue/)) only. |
