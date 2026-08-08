---
title: "Workbook.updateCustomFunctionDefinition"
linktitle: "updateCustomFunctionDefinition"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Updates definition of custom functions."
type: docs
weight: 940
url: /nodejs/aspose.cells/workbook/updatecustomfunctiondefinition/
---

## updateCustomFunctionDefinition(definition)

Updates definition of custom functions. This method can be used for some special scenarios. For example, if user needs some parameters of some custom functions be calculated in array mode, then user may provide their own definition with implemented CustomFunctionDefinition.getArrayModeParameters(java.lang.String) for those functions. After the data of formulas being updated, those specified parameters will be calculated in array mode automatically when calculating corresponding custom functions.

| Parameter | Type | Description |
| --- | --- | --- |
| definition | CustomFunctionDefinition | Special definition of custom functions for user's special requirement. |
