---
title: "FormulaSettings Classe"
linktitle: "FormulaSettings"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe FormulaSettings. Incapsula l'oggetto che rappresenta formulasettings in Go."
type: docs
weight: 200
url: /it/go-cpp/formulasettings/
---

## FormulaSettings class

Impostazioni delle formule e del calcolo.

```go

type FormulaSettings struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetCalculateOnOpen](./getcalculateonopen/) | Indica se l'applicazione deve eseguire un calcolo completo quando la cartella di lavoro viene aperta. |
| [SetCalculateOnOpen](./setcalculateonopen/) | Indica se l'applicazione deve eseguire un calcolo completo quando la cartella di lavoro viene aperta. |
| [GetCalculateOnSave](./getcalculateonsave/) | Indica se ricalcolare la cartella di lavoro prima di salvare il documento, quando è in modalità di calcolo manuale. |
| [SetCalculateOnSave](./setcalculateonsave/) | Indica se ricalcolare la cartella di lavoro prima di salvare il documento, quando è in modalità di calcolo manuale. |
| [GetForceFullCalculation](./getforcefullcalculation/) | Indica se calcola tutte le formule ogni volta che viene avviato un calcolo. |
| [SetForceFullCalculation](./setforcefullcalculation/) | Indica se calcola tutte le formule ogni volta che viene avviato un calcolo. |
| [GetCalculationMode](./getcalculationmode/) | Ottiene o imposta la modalità di calcolo della cartella di lavoro in MS Excel. |
| [SetCalculationMode](./setcalculationmode/) | Ottiene o imposta la modalità di calcolo della cartella di lavoro in MS Excel. |
| [GetCalculationId](./getcalculationid/) | Specifica la versione del motore di calcolo utilizzato per calcolare i valori nella cartella di lavoro. |
| [SetCalculationId](./setcalculationid/) | Specifica la versione del motore di calcolo utilizzato per calcolare i valori nella cartella di lavoro. |
| [GetEnableIterativeCalculation](./getenableiterativecalculation/) | Indica se abilitare il calcolo iterativo per risolvere i riferimenti circolari. |
| [SetEnableIterativeCalculation](./setenableiterativecalculation/) | Indica se abilitare il calcolo iterativo per risolvere i riferimenti circolari. |
| [GetMaxIteration](./getmaxiteration/) | Il numero massimo di iterazioni per risolvere un riferimento circolare. |
| [SetMaxIteration](./setmaxiteration/) | Il numero massimo di iterazioni per risolvere un riferimento circolare. |
| [GetMaxChange](./getmaxchange/) | La variazione massima per risolvere un riferimento circolare. |
| [SetMaxChange](./setmaxchange/) | La variazione massima per risolvere un riferimento circolare. |
| [GetPrecisionAsDisplayed](./getprecisionasdisplayed/) | Indica se la precisione del risultato calcolato deve essere impostata come visualizzata durante il calcolo delle formule. |
| [SetPrecisionAsDisplayed](./setprecisionasdisplayed/) | Indica se la precisione del risultato calcolato deve essere impostata come visualizzata durante il calcolo delle formule. |
| [GetEnableCalculationChain](./getenablecalculationchain/) | Indica se abilitare la catena di calcolo per le formule. Il valore predefinito è false. |
| [SetEnableCalculationChain](./setenablecalculationchain/) | Indica se abilitare la catena di calcolo per le formule. Il valore predefinito è false. |
| [GetPreservePaddingSpaces](./getpreservepaddingspaces/) | Indica se preservare gli spazi e le interruzioni di riga inseriti tra i token delle formule durante il recupero e l'impostazione delle formule. Il valore predefinito è false. |
| [SetPreservePaddingSpaces](./setpreservepaddingspaces/) | Indica se preservare gli spazi e le interruzioni di riga inseriti tra i token delle formule durante il recupero e l'impostazione delle formule. Il valore predefinito è false. |
