---
title: "Classe GlobalizationSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GlobalizationSettings. Rappresenta le impostazioni di globalizzazione"
type: docs
url: /it/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

Rappresenta le impostazioni di globalizzazione.

```csharp
public class GlobalizationSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Ottiene o imposta le impostazioni di globalizzazione per il grafico. |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray/) { get; } | Ottiene il separatore per gli elementi nei dati di riga dell'array nella formula. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator/) { get; } | Ottiene il separatore per l'elenco, i parametri della funzione, ...etc. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Ottiene o imposta le impostazioni di globalizzazione per la tabella pivot. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray/) { get; } | Ottiene il separatore per le righe nei dati dell'array nella formula. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | Confronta due valori stringa secondo determinate regole di ordinamento. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsoleto.**) Ottiene il nome dell'etichetta "(All)" nella PivotTable. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring/)(bool) | Ottiene il valore stringa visualizzato per il valore booleano della cella |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Trasforma la stringa in un oggetto confrontabile secondo determinate regole di ordinamento. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsoleto.**) Ottiene il nome dell'etichetta "Column Labels" nella PivotTable. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename/)(CommentTitleType) | Ottiene il nome del titolo del commento dipendente dalla locale in base al tipo di titolo del commento. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsolete.**) Ottiene il nome dell'intestazione del campo dell'area valori nella Tabella Pivot. |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Ottiene il nome del foglio predefinito per l'aggiunta automatica del foglio di lavoro. Il valore predefinito è "Sheet". |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsolete.**) Ottiene il nome dell'etichetta "(blank)" nella Tabella Pivot. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring/)(string) | Ottiene il valore stringa visualizzato per il valore di errore della cella |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Ottiene il nome del totale generale della funzione. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname/)(string) | Ottiene il testo dipendente dalla locale per il Nome incorporato in base al testo standard fornito. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname/)(string) | Ottiene il nome della funzione dipendente dalla locale in base al nome della funzione standard fornito. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsolete.**) Ottiene il nome dell'etichetta "(Multiple Items)" nella Tabella Pivot. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsolete.**) Ottiene il nome dell'etichetta "Grand Total" nella Tabella Pivot. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsolete.**) Ottiene il nome dell'etichetta "Total" nella Tabella Pivot. È necessario sovrascrivere questo metodo quando la Tabella Pivot contiene due o più PivotField nell'area dati. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsolete.**) Ottiene il nome della protezione nella Tabella Pivot. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsolete.**) Ottiene il nome dell'etichetta "Row Labels" nella Tabella Pivot. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname/)(string) | Ottiene il testo standard del Nome incorporato in base al testo dipendente dalla locale fornito. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname/)(string) | Ottiene il nome standard della funzione in base al nome della funzione dipendente dalla locale fornito. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/)(string) | Ottiene il nome standard dello stile di carattere inglese (Regular, Bold, Italic) per Intestazione/Piè di pagina in base al nome dello stile di carattere locale fornito. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsolete.**) Ottiene il nome del tipo [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) nella Tabella Pivot. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall/)() | Ottiene il nome del tipo di righe della tabella che comprende tutte le righe nella tabella di riferimento. Il valore predefinito è "All", quindi nella formula "#All" rappresenta tutte le righe nella tabella di riferimento. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent/)() | Ottiene il nome del tipo di righe della tabella che comprende la riga corrente nella tabella di riferimento. Il valore predefinito è "This Row", quindi nella formula "#This Row" rappresenta la riga corrente nella tabella di riferimento. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata/)() | Ottiene il nome del tipo di righe della tabella che comprende la regione dati della tabella di riferimento. Il valore predefinito è "Data", quindi nella formula "#Data" rappresenta la regione dati della tabella. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders/)() | Ottiene il nome del tipo di righe della tabella che comprende l'intestazione della tabella. Il valore predefinito è "Headers", quindi nella formula "#Headers" rappresenta l'intestazione della tabella. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals/)() | Ottiene il nome del tipo di righe della tabella che comprende la riga totale della tabella di riferimento. Il valore predefinito è "Totals", quindi nella formula "#Totals" rappresenta la riga totale della tabella di riferimento. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname/)(ConsolidationFunction) | Ottiene il nome totale della funzione. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio
            cells["A1"].PutValue("Region");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("North");
            cells["B2"].PutValue(1000);
            cells["A3"].PutValue("South");
            cells["B3"].PutValue(2000);
            cells["A4"].PutValue("East");
            cells["B4"].PutValue(3000);
            cells["A5"].PutValue("West");
            cells["B5"].PutValue(4000);

            // Crea e applica le impostazioni di globalizzazione
            GlobalizationSettings settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Applica il subtotale con globalizzazione personalizzata
            CellArea area = CellArea.CreateCellArea(0, 0, 5, 1);
            cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 0 }, true, false, true);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetTotalName(ConsolidationFunction functionType)
        {
            // Personalizza il nome totale in base al tipo di funzione
            switch (functionType)
            {
                case ConsolidationFunction.Sum:
                    return "Custom Sum";
                case ConsolidationFunction.Count:
                    return "Custom Count";
                default:
                    return base.GetTotalName(functionType);
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


