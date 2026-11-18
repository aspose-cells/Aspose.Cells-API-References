---
title: "IsParamArrayModeRequired Metod"
linktitle: "IsParamArrayModeRequired"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "IsParamArrayModeRequired-metoden. Inkapslar funktionen som representerar isparamarraymoderequired i Go."
type: docs
weight: 200
url: /sv/go-cpp/abstractcalculationengine/isparamarraymoderequired/
---

## IsParamArrayModeRequired function

Anger om den här motorn behöver att parametern beräknas i arrayläge. Standardvärdet är falskt. Om CalculationData.GetParamValueInArrayMode(int, int, int) krävs vid beräkning av customfunctions och användaren inte har uppdaterat definitionen för dem (via Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)), måste denna egenskap sättas till true.

```go

func (instance *AbstractCalculationEngine) IsParamArrayModeRequired()  (bool,  error) 

```

## Anmärkningar


## Se även

* Class [AbstractCalculationEngine](../)
* Library [Aspose.Cells for Go](../../)
