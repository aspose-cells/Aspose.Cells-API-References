---
title: "Classe PivotGlobalizationSettings"
linktitle: "PivotGlobalizationSettings"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe PivotGlobalizationSettings. Incapsula l'oggetto che rappresenta pivotglobalizationsettings in Go."
type: docs
weight: 200
url: /it/go-cpp/pivotglobalizationsettings/
---

## PivotGlobalizationSettings class

Rappresenta le impostazioni di globalizzazione per le tabelle pivot.

```go

type PivotGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewPivotGlobalizationSettings](./newpivotglobalizationsettings/) | Costruttore predefinito. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetTextOfTotal](./gettextoftotal/) | Ottiene il testo dell'etichetta "Total" nella PivotTable. È necessario sovrascrivere questo metodo quando la PivotTable contiene due o più PivotFields nell'area dati. |
| [GetTextOfGrandTotal](./gettextofgrandtotal/) | Ottiene il testo dell'etichetta "Grand Total" nella PivotTable. |
| [GetTextOfMultipleItems](./gettextofmultipleitems/) | Ottiene il testo dell'etichetta "(Multiple Items)" nella PivotTable. |
| [GetTextOfAll](./gettextofall/) | Ottiene il testo dell'etichetta "(All)" nella PivotTable. |
| [GetTextOfProtectedName](./gettextofprotectedname/) | Ottiene il testo per il nome protetto specificato. |
| [GetTextOfColumnLabels](./gettextofcolumnlabels/) | Ottiene il testo dell'etichetta "Column Labels" nella PivotTable. |
| [GetTextOfRowLabels](./gettextofrowlabels/) | Ottiene il testo dell'etichetta "Row Labels" nella PivotTable. |
| [GetTextOfEmptyData](./gettextofemptydata/) | Ottiene il testo dell'etichetta "(blank)" nella PivotTable. |
| [GetTextOfDataFieldHeader](./gettextofdatafieldheader/) | Ottiene il testo dell'intestazione del campo dell'area valori nella PivotTable. |
| [GetShortTextOf12Months](./getshorttextof12months/) | Ottiene tutte le stringhe brevi formattate dei 12 mesi. |
| [GetTextOf24Hours](./gettextof24hours/) | Ottiene tutte le stringhe formattate localmente delle 24 ore. Il valore predefinito è 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM. |
| [GetTextOfOr](./gettextofor/) | Ottiene tutte le stringhe formattate localmente di "or". |
| [GetFormatOfDayGroup](./getformatofdaygroup/) | Ottiene il formato numerico del gruppo giorno pivot. Utilizzato solo quando si raggruppa il campo pivot per giorni. Il valore predefinito è "d-MMM"; |
| [GetTextOf4Quaters](./gettextof4quaters/) | Ottiene il testo locale di 4 Trimestri. |
| [GetTextOf4Quarters](./gettextof4quarters/) | Ottiene il testo locale di 4 Trimestri. |
| [GetTextOfYears](./gettextofyears/) | Ottiene il testo locale di "Years". |
| [GetTextOfQuarters](./gettextofquarters/) | Ottieni il testo locale di "Quarters". |
| [GetTextOfMonths](./gettextofmonths/) | Ottiene il testo locale di "Months". |
| [GetTextOfDays](./gettextofdays/) | Ottiene il testo locale di "Days". |
| [GetTextOfHours](./gettextofhours/) | Ottiene il testo locale di "Hours". |
| [GetTextOfMinutes](./gettextofminutes/) | Ottiene il testo locale di "Minutes". |
| [GetTextOfSeconds](./gettextofseconds/) | Ottiene il testo locale di "Seconds" |
| [GetTextOfRange](./gettextofrange/) | Ottiene il testo locale di "Range" |
| [GetTextOfAllPeriods](./gettextofallperiods/) | Ottiene il testo locale di "All Periods" |
| [GetTextOfSubTotal](./gettextofsubtotal/) | Ottiene il testo del tipo PivotFieldSubtotalType nella PivotTable. |
| [GetNameOfDataField](./getnameofdatafield/) | Ottiene il nome visualizzato del campo pivot dei dati. Il formato predefinito è "Sum Of Field". |
