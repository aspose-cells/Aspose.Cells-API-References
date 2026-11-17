---
title: "Classe GlobalizationSettings"
linktitle: "GlobalizationSettings"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe GlobalizationSettings. Incapsula l'oggetto che rappresenta globalizationsettings in Go."
type: docs
weight: 200
url: /it/go-cpp/globalizationsettings/
---

## GlobalizationSettings class

Rappresenta le impostazioni di globalizzazione.

```go

type GlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewGlobalizationSettings](./newglobalizationsettings/) | Costruttore predefinito. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetChartSettings](./getchartsettings/) | Ottiene le impostazioni di globalizzazione per Chart. |
| [SetChartSettings](./setchartsettings/) | Imposta le impostazioni di globalizzazione per Chart. |
| [GetPivotSettings](./getpivotsettings/) | Ottiene le impostazioni di globalizzazione per la tabella pivot. |
| [SetPivotSettings](./setpivotsettings/) | Imposta le impostazioni di globalizzazione per la tabella pivot. |
| [GetTotalName](./gettotalname/) | Ottiene il nome totale della funzione. |
| [GetGrandTotalName](./getgrandtotalname/) | Ottiene il nome del totale generale della funzione. |
| [GetDefaultSheetName](./getdefaultsheetname/) | Ottiene il nome predefinito del foglio per aggiungere il foglio di lavoro automaticamente. Il valore predefinito è "Sheet". |
| [GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | Ottiene il nome del tipo di righe della tabella che costituiscono l'intestazione della tabella. Il valore predefinito è "Headers", quindi nella formula "#Headers" rappresenta l'intestazione della tabella. |
| [GetTableRowTypeOfData](./gettablerowtypeofdata/) | Ottiene il nome del tipo di righe della tabella che costituiscono la regione dati della tabella di riferimento. Il valore predefinito è "Data", quindi nella formula "#Data" rappresenta la regione dati della tabella. |
| [GetTableRowTypeOfAll](./gettablerowtypeofall/) | Ottiene il nome del tipo di righe della tabella che comprende tutte le righe nella tabella di riferimento. Il valore predefinito è "All", quindi nella formula "#All" rappresenta tutte le righe nella tabella di riferimento. |
| [GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | Ottiene il nome del tipo di righe della tabella che comprende la riga totale della tabella di riferimento. Il valore predefinito è "Totals", quindi nella formula "#Totals" rappresenta la riga totale della tabella di riferimento. |
| [GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | Ottiene il nome del tipo di righe della tabella che comprende la riga corrente nella tabella di riferimento. Il valore predefinito è "This Row", quindi nella formula "#This Row" rappresenta la riga corrente nella tabella di riferimento. |
| [GetErrorValueString](./geterrorvaluestring/) | Ottiene il valore stringa da visualizzare per il valore di errore della cella |
| [GetBooleanValueString](./getbooleanvaluestring/) | Ottiene il valore stringa da visualizzare per il valore booleano della cella |
| [GetLocalFunctionName](./getlocalfunctionname/) | Ottiene il nome della funzione dipendente dalla locale in base al nome della funzione standard fornito. |
| [GetStandardFunctionName](./getstandardfunctionname/) | Ottiene il nome della funzione standard in base al nome della funzione dipendente dalla locale fornito. |
| [GetLocalBuiltInName](./getlocalbuiltinname/) | Ottiene il testo dipendente dalla locale per il Nome incorporato in base al testo standard fornito. |
| [GetStandardBuiltInName](./getstandardbuiltinname/) | Ottiene il testo standard del Nome incorporato in base al testo dipendente dalla locale fornito. |
| [GetListSeparator](./getlistseparator/) | Ottiene il separatore per elenchi, parametri di funzione, ... ecc. |
| [GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | Ottiene il separatore per le righe nei dati di array nella formula. |
| [GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | Ottiene il separatore per gli elementi nei dati della riga dell'array nella formula. |
| [GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | Ottiene il nome standard dello stile di carattere inglese (Regular, Bold, Italic) per Intestazione/Piè di pagina in base al nome dello stile di carattere locale fornito. |
| [GetCommentTitleName](./getcommenttitlename/) | Ottiene il nome del titolo del commento dipendente dalla locale in base al tipo di titolo del commento. |
| [Compare](./compare/) | Confronta due valori stringa secondo alcune regole di ordinamento. |
