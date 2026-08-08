---
title: "Cell.getDependentsInCalculation"
linktitle: "getDependentsInCalculation"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets all cells whose calculated result depends on this cell."
type: docs
weight: 160
url: /nodejs/aspose.cells/cell/getdependentsincalculation/
---

## getDependentsInCalculation(recursive)

Gets all cells whose calculated result depends on this cell. To use this method, please make sure the workbook has been set with true value for FormulaSettings.EnableCalculationChain and has been fully calculated with this setting. If there is no formula reference to this cell, null will be returned.

| Parameter | Type | Description |
| --- | --- | --- |
| recursive | boolean | Whether returns those dependents which do not reference to this cell directly but reference to other leafs of this cell |

**Returns:** Iterator — `Iterator` Enumerator to enumerate all dependents(Cell objects)
