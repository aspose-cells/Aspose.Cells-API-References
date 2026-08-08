---
title: "Cells.getDependentsInCalculation"
linktitle: "getDependentsInCalculation"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets all cells whose calculated result depends on specific cell."
type: docs
weight: 660
url: /nodejs/aspose.cells/cells/getdependentsincalculation/
---

## getDependentsInCalculation(row, column, recursive)

Gets all cells whose calculated result depends on specific cell. To use this method, please make sure the workbook has been set with true value for FormulaSettings.EnableCalculationChain and has been fully calculated with this setting. If there is no formula reference to this cell, null will be returned. For more details and example, please see Cell.getDependentsInCalculation(boolean)

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | Row index of the specific cell |
| column | Number | Column index of the specific cell. |
| recursive | boolean | Whether returns those dependents which do not reference to the specific cell directly but reference to other leafs of that cell. |

**Returns:** Iterator — `Iterator` Enumerator to enumerate all dependents(Cell objects)
