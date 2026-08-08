---
title: "FormulaSettings.setCalculationId"
linktitle: "setCalculationId"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Specifies the version of the calculation engine used to calculate values in the workbook."
type: docs
weight: 140
url: /nodejs/aspose.cells/formulasettings/setcalculationid/
---

## setCalculationId()

Specifies the version of the calculation engine used to calculate values in the workbook. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. In the case of ms excel, if the value of this property is less than the recalculation engine identifier associated with the application that opens the resultant file, the application will recalculate the results of all formulas on this workbook immediately after loading the file. For performance consideration for most users' applications, we do not calculate any formula on the workbook automatically, no matter what value has been set for this property.
