---
title: "CalculationData.getCell"
linktitle: "getCell"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets the Cell object where the function is in."
type: docs
weight: 20
url: /nodejs/aspose.cells/calculationdata/getcell/
---

## getCell()

Gets the Cell object where the function is in. When calculating a formula without setting it to a cell, such as by Worksheet.calculateFormula(java.lang.String, com.aspose.cells.CalculationOptions), the formula will be calculated just like it has been set to cell A1, so both CellRow and CellColumn are 0. However, cell A1 in the worksheet may has not been instantiated. So for such kind of situation this property will be null.
