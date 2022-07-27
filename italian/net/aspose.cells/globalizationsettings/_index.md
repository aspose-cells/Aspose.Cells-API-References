---
title: GlobalizationSettings
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta le impostazioni di globalizzazione.
type: docs
weight: 3620
url: /it/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

Rappresenta le impostazioni di globalizzazione.

```csharp
public class GlobalizationSettings : AbstractGlobalizationSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GlobalizationSettings](globalizationsettings)() | Default_Costruttore |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings) { get; set; } | Ottiene o imposta il grafico di questo[`ChartGlobalizationSettings`](../../aspose.cells.charts/chartglobalizationsettings) |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray) { get; } | Ottiene il separatore per gli elementi nei dati di riga dell'array nella formula. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator) { get; } | Ottiene il separatore per elenco, parametri di funzione, ...ecc. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray) { get; } | Ottiene il separatore per le righe nei dati dell'array nella formula. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare)(string, string, bool) | Confronta due valori di stringa in base a determinate regole di confronto. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname)() | Ottiene il nome dell'etichetta "(Tutto)" nella tabella pivot. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring)(bool) | Ottiene il valore della stringa di visualizzazione per il valore booleano della cella |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey)(string, bool) | Trasforma la stringa in un oggetto comparabile in base a determinate regole di confronto. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable)() | Ottiene il nome dell'etichetta "Etichette colonne" nella tabella pivot. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename)(CommentTitleType) | Ottiene il nome del titolo del commento dipendente dalla locale in base al tipo di titolo del commento. |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname)() | Ottiene il nome dell'etichetta "(vuoto)" nella tabella pivot. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring)(string) | Ottiene il valore della stringa di visualizzazione per il valore di errore della cella |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname)(ConsolidationFunction) | Ottiene il nome del totale generale della funzione. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname)(string) | Ottiene il testo dipendente dalla locale per il nome integrato in base al testo standard specificato. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname)(string) | Ottiene il nome della funzione dipendente dalla locale in base al nome della funzione standard specificato. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname)() | Ottiene il nome dell'etichetta "(elementi multipli)" nella tabella pivot. |
| virtual [GetOtherName](../../aspose.cells/globalizationsettings/getothername)() | Ottiene il nome delle etichette "Altro" per i grafici a torta. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname)() | Ottiene il nome dell'etichetta "Totale generale" nella tabella pivot. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname)() | Ottiene il nome dell'etichetta "Total" nella tabella pivot. È necessario ignorare questo metodo quando la tabella pivot contiene due o più campi pivot nell'area dati. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable)() | Ottiene il nome della protezione nella tabella pivot. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable)() | Ottiene il nome dell'etichetta "Etichette di riga" nella tabella pivot. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname)(string) | Ottiene il testo standard del nome integrato in base al testo dipendente dalla locale specificato. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname)(string) | Ottiene il nome della funzione standard in base al nome della funzione dipendente dalla locale specificata. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename)(string) | Ottiene il nome dello stile del carattere inglese standard (normale, grassetto, corsivo) per l'intestazione/piè di pagina in base al nome dello stile del carattere locale specificato. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname)(PivotFieldSubtotalType) | Ottiene il nome di[`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype) digita nella tabella pivot. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall)() | Ottiene il nome del tipo delle righe della tabella che consiste di tutte le righe nella tabella di riferimento. Il valore predefinito è "Tutto", quindi nella formula "#Tutto" rappresenta tutte le righe nella tabella di riferimento. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent)() | Ottiene il nome del tipo delle righe della tabella che consiste nella riga corrente nella tabella di riferimento. Il valore predefinito è "Questa riga", quindi nella formula "#Questa riga" rappresenta la riga corrente nella tabella di riferimento. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata)() | Ottiene il nome del tipo delle righe della tabella che consiste nell'area dati della tabella di riferimento. L'impostazione predefinita è "Dati", quindi nella formula "#Dati" rappresenta l'area dati della tabella. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders)() | Ottiene il nome del tipo delle righe della tabella che consiste nell'intestazione della tabella. Il valore predefinito è "Intestazioni", quindi nella formula "#Intestazioni" rappresenta l'intestazione della tabella. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals)() | Ottiene il nome del tipo delle righe della tabella che consiste nella riga totale della tabella di riferimento. L'impostazione predefinita è "Totali", quindi nella formula "#Totali" rappresenta la riga totale della tabella di riferimento. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname)(ConsolidationFunction) | Ottiene il nome totale della funzione. |

### Guarda anche

* class [AbstractGlobalizationSettings](../abstractglobalizationsettings)
* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
