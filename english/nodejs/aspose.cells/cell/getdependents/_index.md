---
title: "Cell.getDependents"
linktitle: "getDependents"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Get all cells whose formula references to this cell directly."
type: docs
weight: 150
url: /nodejs/aspose.cells/cell/getdependents/
---

## getDependents(isAll)

Get all cells whose formula references to this cell directly. If one reference containing this cell appears in one cell's formula, that cell will be taken as the dependent of this cell, no matter the reference or this cell is used or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, this formula is still be taken as A2's dependent. To get those formulas whose calculated results depend on this cell, please use getDependentsInCalculation(boolean).When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked. So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will cause poor performance. For performance consideration, user should use getDependentsInCalculation(boolean) instead. Or, user may gather precedents map of all cells by getPrecedents() firstly, and then build the dependents map according to the precedents map.

| Parameter | Type | Description |
| --- | --- | --- |
| isAll | boolean | Indicates whether check formulas in other worksheets |
