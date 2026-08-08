---
title: "CalculationData.getCalculatedValue"
linktitle: "getCalculatedValue"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets or sets the calculated value for this function."
type: docs
weight: 10
url: /nodejs/aspose.cells/calculationdata/getcalculatedvalue/
---

## getCalculatedValue()

Gets or sets the calculated value for this function. User should set this property in his custom calculation engine for those functions the engine supports, and the set value will be returned when getting this property later. The set value may be of possible types of Cell.Value, or array of such kind of values, or a Range, Name, ReferredArea. Getting this property before setting value to it will make the function be calculated by the default calculation engine of Aspose.Cells and then the calculated value will be returned(generally it should be #NAME? for user-defined functions).
