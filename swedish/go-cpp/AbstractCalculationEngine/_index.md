---
title: "AbstractCalculationEngine klass"
linktitle: "AbstractCalculationEngine"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "AbstractCalculationEngine klass. Inkapslar objektet som representerar abstractcalculationengine i Go."
type: docs
weight: 200
url: /sv/go-cpp/abstractcalculationengine/
---

## AbstractCalculationEngine class

Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn i Aspose.Cells.

```go

type AbstractCalculationEngine struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [SkipCalculation](./skipcalculation/) | Hoppar över beräkningen för hela formeln som refererar till funktionen som för närvarande utvärderas. |
| [IsParamLiteralRequired](./isparamliteralrequired/) | Anger om den här motorn behöver den bokstavliga texten för parametern under en beräkning. Standardvärdet är falskt. |
| [IsParamArrayModeRequired](./isparamarraymoderequired/) | Anger om den här motorn behöver att parametern beräknas i arrayläge. Standardvärdet är falskt. Om CalculationData.GetParamValueInArrayMode(int, int, int) krävs vid beräkning av customfunctions och användaren inte har uppdaterat definitionen för dem (via Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)), måste denna egenskap sättas till true. |
| [GetProcessBuiltInFunctions](./getprocessbuiltinfunctions/) | Om inbyggda funktioner som har stöd av den inbyggda motorn ska kontrolleras och bearbetas av denna implementation. Standard är falskt. |
| [ForceRecalculate](./forcerecalculate/) | Om den angivna funktionen ska tvingas att alltid beräknas om vid beräkning av delade formler. |
