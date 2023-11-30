---
title: Aspose::Cells::Cell::SetDynamicArrayFormula method
linktitle: SetDynamicArrayFormula
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Cell::SetDynamicArrayFormula method. Sets dynamic array formula and make the formula spill into neighboring cells if possible in C++.'
type: docs
weight: 5100
url: /cpp/aspose.cells/cell/setdynamicarrayformula/
---
## Cell::SetDynamicArrayFormula(const U16String\&, const FormulaParseOptions\&, bool) method


Sets dynamic array formula and make the formula spill into neighboring cells if possible.

```cpp
CellArea Aspose::Cells::Cell::SetDynamicArrayFormula(const U16String &arrayFormula, const FormulaParseOptions &options, bool calculateValue)
```


| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | const U16String\& | the formula expression |
| options | const FormulaParseOptions\& | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| calculateValue | bool | whether calculate this dynamic array formula for those cells in the spilled range. |

## ReturnValue

the range that the formula should spill into.

## See Also

* Class [CellArea](../../cellarea/)
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::SetDynamicArrayFormula(const char16_t*, const FormulaParseOptions\&, bool) method


Sets dynamic array formula and make the formula spill into neighboring cells if possible.

```cpp
CellArea Aspose::Cells::Cell::SetDynamicArrayFormula(const char16_t *arrayFormula, const FormulaParseOptions &options, bool calculateValue)
```


| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | const char16_t* | the formula expression |
| options | const FormulaParseOptions\& | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| calculateValue | bool | whether calculate this dynamic array formula for those cells in the spilled range. |

## ReturnValue

the range that the formula should spill into.

## See Also

* Class [CellArea](../../cellarea/)
* Class [Vector](../../vector/)
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
