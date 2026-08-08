---
title: "FormulaSettings.getCalculationMode"
linktitle: "getCalculationMode"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets or sets the mode for workbook calculation in ms excel."
type: docs
weight: 40
url: /nodejs/aspose.cells/formulasettings/getcalculationmode/
---

## getCalculationMode()

Gets or sets the mode for workbook calculation in ms excel. The value of the property is CalcModeType integer constant. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most user's application, we do not calculate any formula in the workbook automatically, no matter what mode has been set for this property. If user needs to calculate formulas, please always call methods on different objects according to requirement: Workbook.calculateFormula(), Worksheet.calculateFormula(com.aspose.cells.CalculationOptions, boolean), Cell.calculate(com.aspose.cells.CalculationOptions), ...etc.
