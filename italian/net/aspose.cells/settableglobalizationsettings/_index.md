---
title: "Classe SettableGlobalizationSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.SettableGlobalizationSettings. Implementazione di GlobalizationSettings che consente all'utente di impostare/modificare i testi predefiniti"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/
---
## SettableGlobalizationSettings class

Implementazione di GlobalizationSettings che consente all'utente di impostare/modificare testi predefiniti.

```csharp
public class SettableGlobalizationSettings : GlobalizationSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SettableGlobalizationSettings](settableglobalizationsettings/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Ottiene o imposta le impostazioni di globalizzazione per Chart.(Ereditato da [`GlobalizationSettings`](../globalizationsettings/).) |
| override [ColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/) { get; } | Ottiene il separatore per gli elementi nei dati di riga dell'array nella formula. |
| override [ListSeparator](../../aspose.cells/settableglobalizationsettings/listseparator/) { get; } | Ottiene il separatore per l'elenco, i parametri della funzione, ...etc. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Ottiene o imposta le impostazioni di globalizzazione per la tabella pivot.(Ereditato da [`GlobalizationSettings`](../globalizationsettings/).) |
| override [RowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/) { get; } | Ottiene il separatore per le righe nei dati dell'array nella formula. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | Confronta due valori stringa secondo determinate regole di ordinamento.(Ereditato da [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsoleto.**) Ottiene il nome dell'etichetta "(All)" nella Tabella Pivot.(Ereditato da [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetBooleanValueString](../../aspose.cells/settableglobalizationsettings/getbooleanvaluestring/)(bool) | Ottiene il valore stringa visualizzato per il valore booleano della cella |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Trasforma la stringa in un oggetto confrontabile secondo determinate regole di ordinamento.(Ereditato da [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsoleto.**) Ottiene il nome dell'etichetta "Column Labels" nella Tabella Pivot.(Ereditato da [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetCommentTitleName](../../aspose.cells/settableglobalizationsettings/getcommenttitlename/)(CommentTitleType) | Ottiene il nome del titolo del commento dipendente dalla locale in base al tipo di titolo del commento. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsoleto.**) Ottiene il nome dell'intestazione del campo dell'area valori nella Tabella Pivot.(Ereditato da [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Ottiene il nome foglio predefinito per aggiungere automaticamente un foglio di lavoro. Il valore predefinito è "Sheet".(Ereditato da [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsoleto.**) Ottiene il nome dell'etichetta "(blank)" nella Tabella Pivot.(Ereditato da [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetErrorValueString](../../aspose.cells/settableglobalizationsettings/geterrorvaluestring/)(string) | Ottiene il valore stringa visualizzato per il valore di errore della cella |
| override [GetGrandTotalName](../../aspose.cells/settableglobalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Ottiene il nome del totale generale della funzione. |
| override [GetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/getlocalbuiltinname/)(string) | Ottiene il testo dipendente dalla locale per il Nome incorporato in base al testo standard fornito. |
| override [GetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/getlocalfunctionname/)(string) | Ottiene il nome della funzione dipendente dalla locale in base al nome della funzione standard fornito. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsoleto.**) Ottiene il nome dell'etichetta "(Multiple Items)" nella Tabella Pivot.(Ereditato da [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsoleto.**) Ottiene il nome dell'etichetta "Grand Total" nella Tabella Pivot.(Ereditato da [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsoleto.**) Ottiene il nome dell'etichetta "Total" nella Tabella Pivot. È necessario sovrascrivere questo metodo quando la Tabella Pivot contiene due o più PivotField nell'area dati.(Ereditato da [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsoleto.**) Ottiene il nome della protezione nella Tabella Pivot.(Ereditato da [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsoleto.**) Ottiene il nome dell'etichetta "Row Labels" nella Tabella Pivot.(Ereditato da [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/getstandardbuiltinname/)(string) | Ottiene il testo standard del Nome incorporato in base al testo dipendente dalla locale fornito. |
| override [GetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/getstandardfunctionname/)(string) | Ottiene il nome standard della funzione in base al nome della funzione dipendente dalla locale fornito. |
| override [GetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/)(string) | Ottiene il nome standard dello stile di carattere inglese (Regular, Bold, Italic) per Intestazione/Piè di pagina in base al nome dello stile di carattere locale fornito. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsoleto.**) Ottiene il nome del tipo [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) nella Tabella Pivot.(Ereditato da [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofall/)() | Ottiene il nome del tipo di righe della tabella che comprende tutte le righe nella tabella di riferimento. |
| override [GetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofcurrent/)() | Ottiene il nome del tipo di righe della tabella che comprende la riga corrente nella tabella di riferimento. |
| override [GetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofdata/)() | Ottiene il nome del tipo di righe della tabella che comprende la regione dati della tabella di riferimento. Il valore predefinito è "Data", quindi nella formula "#Data" rappresenta la regione dati della tabella. |
| override [GetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofheaders/)() | Ottiene il nome del tipo di righe della tabella che comprende l'intestazione della tabella. Il valore predefinito è "Headers", quindi nella formula "#Headers" rappresenta l'intestazione della tabella. |
| override [GetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/gettablerowtypeoftotals/)() | Ottiene il nome del tipo delle righe della tabella che consiste nella riga totale della tabella di riferimento. |
| override [GetTotalName](../../aspose.cells/settableglobalizationsettings/gettotalname/)(ConsolidationFunction) | Ottiene il nome totale della funzione specifica. |
| [SetBooleanValueString](../../aspose.cells/settableglobalizationsettings/setbooleanvaluestring/)(bool, string) | Imposta il valore stringa di visualizzazione per il valore booleano della cella |
| [SetColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/)(char) | Imposta il separatore per gli elementi nei dati della riga dell'array nella formula. |
| [SetCommentTitleName](../../aspose.cells/settableglobalizationsettings/setcommenttitlename/)(CommentTitleType, string) | Ottiene il nome del titolo del commento dipendente dalla locale in base al tipo di titolo del commento. |
| [SetGrandTotalName](../../aspose.cells/settableglobalizationsettings/setgrandtotalname/)(ConsolidationFunction, string) | Imposta il nome del totale complessivo della funzione specifica. |
| [SetListSeparator](../../aspose.cells/settableglobalizationsettings/setlistseparator/)(char) | Imposta il separatore per l'elenco, i parametri della funzione, ...ecc. |
| [SetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/setlocalbuiltinname/)(string, string, bool) | Imposta il testo dipendente dalla locale per il nome integrato con il testo del nome standard fornito. |
| [SetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/setlocalfunctionname/)(string, string, bool) | Imposta il nome della funzione dipendente dalla locale corrispondente al nome della funzione standard fornito. |
| [SetRowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/)(char) | Imposta il separatore per le righe nei dati dell'array nella formula. |
| [SetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/setstandardbuiltinname/)(string, string, bool) | Imposta il nome della funzione dipendente dalla locale secondo il nome della funzione standard fornito. |
| [SetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/setstandardfunctionname/)(string, string, bool) | Imposta il nome della funzione dipendente dalla locale secondo il nome della funzione standard fornito. |
| [SetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/)(string, string) | Imposta il nome della funzione dipendente dalla locale secondo il nome della funzione standard fornito. |
| [SetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/settablerowtypeofall/)(string) | Imposta il nome del tipo delle righe della tabella che consiste in tutte le righe della tabella di riferimento. |
| [SetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/)(string) | Imposta il nome del tipo delle righe della tabella che consiste nella riga corrente della tabella di riferimento. |
| [SetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/settablerowtypeofdata/)(string) | Imposta il nome del tipo delle righe della tabella che consiste nella regione dati della tabella di riferimento. |
| [SetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/)(string) | Imposta il nome del tipo delle righe della tabella che consiste nell'intestazione della tabella. |
| [SetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/)(string) | Imposta il nome del tipo delle righe della tabella che consiste nella riga totale della tabella di riferimento. |
| [SetTotalName](../../aspose.cells/settableglobalizationsettings/settotalname/)(ConsolidationFunction, string) | Imposta il nome totale della funzione specifica. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;

    public class CellsClassSettableGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Imposta il separatore personalizzato per l'elenco
            settings.SetListSeparator(';');

            // Imposta le stringhe personalizzate per i valori booleani
            settings.SetBooleanValueString(true, "TRUE_CUSTOM");
            settings.SetBooleanValueString(false, "FALSE_CUSTOM");

            // Imposta i nomi personalizzati delle funzioni
            settings.SetLocalFunctionName("SUM", "SUMME", true);
            settings.SetLocalFunctionName("AVERAGE", "MITTELWERT", true);

            // Imposta i nomi personalizzati dei tipi di riga della tabella
            settings.SetTableRowTypeOfHeaders("HEADERS_CUSTOM");
            settings.SetTableRowTypeOfData("DATA_CUSTOM");
            settings.SetTableRowTypeOfTotals("TOTALS_CUSTOM");

            // Imposta i nomi personalizzati dei titoli dei commenti
            settings.SetCommentTitleName(CommentTitleType.Comment, "COMMENT_CUSTOM");
            // Rimossa la riga Author poiché CommentTitleType non ha quel valore enum
            // Se è necessario impostare le impostazioni relative all'autore, è necessario utilizzare ThreadedCommentAuthor

            // Applica le impostazioni di globalizzazione al workbook
            workbook.Settings.GlobalizationSettings = settings;

            // Dimostrare l'utilizzo nelle formule
            worksheet.Cells["A1"].Formula = "=TRUE()";
            worksheet.Cells["A2"].Formula = "=FALSE()";
            worksheet.Cells["A3"].Formula = "=SUM(1,2,3)";
            worksheet.Cells["A4"].Formula = "=AVERAGE(1,2,3)";

            // Salva la cartella di lavoro
            workbook.Save("SettableGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../globalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


