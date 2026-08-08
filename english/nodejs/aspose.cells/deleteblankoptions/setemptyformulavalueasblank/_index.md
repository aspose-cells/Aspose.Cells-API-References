---
title: "DeleteBlankOptions.setEmptyFormulaValueAsBlank"
linktitle: "setEmptyFormulaValueAsBlank"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string."
type: docs
weight: 110
url: /nodejs/aspose.cells/deleteblankoptions/setemptyformulavalueasblank/
---

## setEmptyFormulaValueAsBlank()

Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false. Generally user should make sure the formulas have been calculated before deleting operation with this property as true. Otherwise all newly cretaed formulas by normal apis such as Cell.Formula will be taken as blank and may be deleted because before calculation their calculated results are all null.
