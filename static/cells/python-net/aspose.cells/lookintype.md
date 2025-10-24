##LookInType enumeration
## LookInType enumeration
Represents look in type.
The LookInType type exposes the following members:
### Fields
| Field | Description |
| :- | :- |
| FORMULAS | Finds the searched object from formula([`Cell.formula`](/cells/python-net/aspose.cells/cell#formula)) if the cell is formula,
| VALUES | Finds object from cell's original value([`Cell.value`](/cells/python-net/aspose.cells/cell#value))
| VALUES_EXCLUDE_FORMULA_CELL | Ignores cells that are formula. For those cells that are not formula,
| COMMENTS | Finds object from cell's comment only. Ignores those cells that have no comment. |
| ONLY_FORMULAS | Ignores cells that are not formula. For those cells that are formula,
| ORIGINAL_VALUES | Find object from cell's original value only. |
| FORMATTED_VALUES | Find object from cell's formatted value([`Cell.string_value`](/cells/python-net/aspose.cells/cell#string_value)) only. |
### See Also
* module [`aspose.cells`](..)
