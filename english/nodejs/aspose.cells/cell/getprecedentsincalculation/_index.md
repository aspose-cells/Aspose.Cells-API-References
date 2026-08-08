---
title: "Cell.getPrecedentsInCalculation"
linktitle: "getPrecedentsInCalculation"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it."
type: docs
weight: 380
url: /nodejs/aspose.cells/cell/getprecedentsincalculation/
---

## getPrecedentsInCalculation()

Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it. This method can only work with the situation that FormulaSettings.EnableCalculationChain is true for the workbook and the workbook has been fully calculated. If this cell is not a formula or it does not reference to any other cells, null will be returned.

**Returns:** Iterator — `Iterator` Enumerator to enumerate all references(ReferredArea)
