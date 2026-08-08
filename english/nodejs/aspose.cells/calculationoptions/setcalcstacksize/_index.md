---
title: "CalculationOptions.setCalcStackSize"
linktitle: "setCalcStackSize"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "The stack size for calculating cells recursively."
type: docs
weight: 110
url: /nodejs/aspose.cells/calculationoptions/setcalcstacksize/
---

## setCalcStackSize()

The stack size for calculating cells recursively. Default value is 200. When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.
