---
title: "Classe AbstractCalculationEngine"
linktitle: "AbstractCalculationEngine"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe AbstractCalculationEngine. Incapsula l'oggetto che rappresenta abstractcalculationengine in Go."
type: docs
weight: 200
url: /it/go-cpp/abstractcalculationengine/
---

## AbstractCalculationEngine class

Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di Aspose.Cells.

```go

type AbstractCalculationEngine struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [SkipCalculation](./skipcalculation/) | Salta il calcolo per l'intera formula che fa riferimento alla funzione attualmente in valutazione. |
| [IsParamLiteralRequired](./isparamliteralrequired/) | Indica se questo motore necessita del testo letterale del parametro durante il calcolo. Il valore predefinito è false. |
| [IsParamArrayModeRequired](./isparamarraymoderequired/) | Indica se questo motore necessita che il parametro sia calcolato in modalità array. Il valore predefinito è false. Se CalculationData.GetParamValueInArrayMode(int, int, int) è richiesto durante il calcolo di customfunctions e l'utente non ha aggiornato la definizione per esse (tramite Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)), questa proprietà deve essere impostata su true. |
| [GetProcessBuiltInFunctions](./getprocessbuiltinfunctions/) | Indica se le funzioni integrate supportate dal motore integrato debbano essere verificate ed elaborate da questa implementazione. Il valore predefinito è false. |
| [ForceRecalculate](./forcerecalculate/) | Indica se forzare la ricalcolazione della funzione fornita ogni volta durante il calcolo delle formule condivise. |
