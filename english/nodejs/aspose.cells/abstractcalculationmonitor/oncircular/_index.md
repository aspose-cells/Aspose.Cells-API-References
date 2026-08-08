---
title: "AbstractCalculationMonitor.onCircular"
linktitle: "onCircular"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Implement this method to do business when calculating formulas with circular references."
type: docs
weight: 60
url: /nodejs/aspose.cells/abstractcalculationmonitor/oncircular/
---

## onCircular(circularCellsData)

Implement this method to do business when calculating formulas with circular references. In the implementation user may also set the expected value as calculated result for part/all of those cells so the formula engine will not calculate them recursively.

| Parameter | Type | Description |
| --- | --- | --- |
| circularCellsData | Iterator | IEnumerator with |

**Returns:** boolean — `boolean` Whether the formula engine needs to calculate those cells in circular after this call. True to let the formula engine continue to do calculation for them. False to let the formula engine just mark those cells as Calculated.
