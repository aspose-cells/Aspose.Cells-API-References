---
title: FormulaParseOptions
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 710
url: /python-net/aspose.cells/formulaparseoptions/
---

## FormulaParseOptions class

Represents options when parsing formula.

The FormulaParseOptions type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|FormulaParseOptions()|Initializes a new instance of the FormulaParseOptions class|
## Properties
| Name | Description |
| :- | :- |
|locale_dependent|Whether the formula is locale formatted. Default is false.|
|r1c1_style|Whether the formula is R1C1 reference style. Default is false.|
|check_add_in|Whether check addins in existing external links of current workbook for user defined function without external link.<br/>            Default is true(if user defined function matches one addin in existing external links, then take it as the addin).|
|parse|Whether parse given formula. Default is true.<br/>            If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them<br/>            or parsed formula data is required by other operations such as calculating formulas.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)
