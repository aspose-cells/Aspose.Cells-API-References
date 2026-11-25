---
title: "Classe PivotField"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Pivot.PivotField. Rappresenta un campo in un report PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/
---
## PivotField class

Rappresenta un campo in un report PivotTable.

```csharp
public class PivotField : IDisposable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AllowDraggingToColumn](../../aspose.cells.pivot/pivotfield/allowdraggingtocolumn/) { get; set; } | Indica se il campo specificato può essere trascinato nella regione colonna. Il valore predefinito è true. |
| [AllowDraggingToData](../../aspose.cells.pivot/pivotfield/allowdraggingtodata/) { get; set; } | Indica se il campo specificato può essere trascinato nella regione valori. Il valore predefinito è true. |
| [AllowDraggingToPage](../../aspose.cells.pivot/pivotfield/allowdraggingtopage/) { get; set; } | Indica se il campo specificato può essere trascinato nella regione pagina. Il valore predefinito è true. |
| [AllowDraggingToRow](../../aspose.cells.pivot/pivotfield/allowdraggingtorow/) { get; set; } | Indica se il campo specificato può essere trascinato nella regione riga. Il valore predefinito è true. |
| [AllowRemovingFromView](../../aspose.cells.pivot/pivotfield/allowremovingfromview/) { get; set; } | Indica se questo campo pivot può essere rimosso dalla visualizzazione PivotTable. Il valore predefinito è true. |
| [AutoShowCount](../../aspose.cells.pivot/pivotfield/autoshowcount/) { get; set; } | (**Obsolete.**) Rappresenta il numero di elementi superiori o inferiori visualizzati automaticamente nel campo PivotTable specificato. |
| [AutoShowField](../../aspose.cells.pivot/pivotfield/autoshowfield/) { get; set; } | (**Obsolete.**) Rappresenta l'indice del campo di visualizzazione automatica. -1 indica il PivotField stesso. Deve essere l'indice dei campi dati. |
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield/) { get; set; } | (**Obsolete.**) Rappresenta l'indice del campo ordinato automaticamente. -1 indica il PivotField stesso, gli altri indicano la posizione dei campi dati. |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex/) { get; set; } | Rappresenta l'indice nei campi pivot di origine. |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem/) { get; set; } | Ottiene o imposta l'elemento di pagina attualmente visualizzato per questo campo pivot (solo campo pagina). |
| [CurrentPageItemText](../../aspose.cells.pivot/pivotfield/currentpageitemtext/) { get; set; } | Ottiene il testo visualizzato dell'elemento di pagina corrente per questo campo pivot (solo campo pagina). |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname/) { get; set; } | Rappresenta il nome visualizzato del campo pivot nella visualizzazione della tabella pivot. |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn/) { get; set; } | (**Obsolete.**) Indica se il campo specificato può essere trascinato nella regione colonne. Il valore predefinito è true. |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata/) { get; set; } | (**Obsolete.**) Indica se il campo specificato può essere trascinato nella regione valori. Il valore predefinito è true. |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide/) { get; set; } | (**Obsolete.**) Indica se questo campo pivot può essere rimosso dalla visualizzazione della PivotTable. Il valore predefinito è true. |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage/) { get; set; } | (**Obsolete.**) Indica se il campo specificato può essere trascinato nella regione pagina. Il valore predefinito è true. |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow/) { get; set; } | (**Obsolete.**) Indica se il campo specificato può essere trascinato nella regione righe. Il valore predefinito è true. |
| [Function](../../aspose.cells.pivot/pivotfield/function/) { get; set; } | Rappresenta la funzione utilizzata per riepilogare questo campo dati della PivotTable. |
| [GroupSettings](../../aspose.cells.pivot/pivotfield/groupsettings/) { get; } | Ottiene le impostazioni di raggruppamento del campo pivot. |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow/) { get; set; } | Indica se inserire una riga vuota dopo ogni elemento. Solo per i campi riga. |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow/) { get; set; } | (**Obsolete.**) Indica se il campo PivotTable specificato è visualizzato automaticamente in ordine ascendente. |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort/) { get; set; } | (**Obsolete.**) Indica se gli elementi di questo campo pivot sono ordinati automaticamente in ordine ascendente. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow/) { get; set; } | (**Obsolete.**) Indica se il campo PivotTable specificato è mostrato automaticamente. |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort/) { get; set; } | (**Obsolete.**) Indica se gli elementi di questo campo PivotTable sono ordinati automaticamente. |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals/) { get; set; } | Indica se il campo specificato mostra subtotali automatici. Il valore predefinito è true. |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield/) { get; } | Indica se questo campo pivot è un campo calcolato. |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter/) { get; set; } | Indica se includere nuovi elementi nel campo nel filtro manuale. Il valore predefinito è false. |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems/) { get; set; } | Indica se inserire interruzioni di pagina dopo ogni elemento. Il valore predefinito è false. |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed/) { get; set; } | Indica se è possibile selezionare più elementi nel campo pagina. Il valore predefinito è false. |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels/) { get; set; } | Indica se ripetere le etichette del campo nella regione riga o colonna. Il valore predefinito è false. |
| [IsValueFields](../../aspose.cells.pivot/pivotfield/isvaluefields/) { get; } | (**Obsolete.**) Indica se questo campo rappresenta campi di valori. |
| [IsValuesField](../../aspose.cells.pivot/pivotfield/isvaluesfield/) { get; } | Indica se questo campo rappresenta un campo di valori. |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount/) { get; } | (**Obsolete.**) Ottiene il conteggio degli elementi base in questo campo pivot. |
| [Items](../../aspose.cells.pivot/pivotfield/items/) { get; } | Ottieni tutte le etichette degli elementi pivot in questo campo. |
| [Name](../../aspose.cells.pivot/pivotfield/name/) { get; set; } | Rappresenta il nome di PivotField. |
| [NonAutoSortDefault](../../aspose.cells.pivot/pivotfield/nonautosortdefault/) { get; set; } | (**Obsolete.**) Indica se un'operazione di ordinamento che verrà applicata a questo campo pivot è un'operazione di autosort o un semplice ordinamento dei dati. |
| [Number](../../aspose.cells.pivot/pivotfield/number/) { get; set; } | Rappresenta il formato di visualizzazione predefinito di numeri e date. |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat/) { get; set; } | Rappresenta il formato di visualizzazione personalizzato di numeri e date. |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems/) { get; } | Ottieni gli elementi base originali; |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems/) { get; } | Ottiene gli elementi pivot del campo pivot |
| [Position](../../aspose.cells.pivot/pivotfield/position/) { get; } | Rappresenta l'indice di `PivotField` nella regione. |
| [RegionType](../../aspose.cells.pivot/pivotfield/regiontype/) { get; } | Specifica la regione della tabella pivot in cui viene visualizzato questo campo. |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems/) { get; set; } | Indica se visualizzare tutti gli elementi nella vista PivotTable, anche se non contengono dati di riepilogo. Il valore predefinito è false. |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact/) { get; set; } | (**Obsolete.**) Indica se visualizzare le etichette del campo successivo nella stessa colonna nella vista Pivot Table. Solo per i campi di riga. |
| [ShowInCompactForm](../../aspose.cells.pivot/pivotfield/showincompactform/) { get; set; } | Ottiene o imposta un valore che indica se questo campo di riga utilizza il layout a forma compatta. Si applica solo ai campi di riga. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform/) { get; set; } | Ottiene o imposta un valore che indica se questo campo di riga utilizza il layout a contorno. Si applica solo ai campi di riga. |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop/) { get; set; } | Indica se visualizzare i subtotali in alto o in basso degli elementi. |
| [ShowValuesSetting](../../aspose.cells.pivot/pivotfield/showvaluessetting/) { get; } | Ottiene le impostazioni per mostrare i valori quando è in uso il calcolo ShowDataAs. |
| [SortSetting](../../aspose.cells.pivot/pivotfield/sortsetting/) { get; } | Ottiene tutte le impostazioni di ordinamento automatico |
| [Subtotals](../../aspose.cells.pivot/pivotfield/subtotals/) { get; set; } | Ottiene o imposta i subtotali del campo. Solo per i campi pivot di riga o colonna. |
| [Top10AutoShowSettings](../../aspose.cells.pivot/pivotfield/top10autoshowsettings/) { get; } | Ottiene le impostazioni Top 10 AutoShow per un campo pivot. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem/)(string, string) | Aggiunge un elemento formula calcolata al campo pivot. |
| [ClearFilter](../../aspose.cells.pivot/pivotfield/clearfilter/)() | Cancella le impostazioni del filtro su questo campo pivot. |
| [Dispose](../../aspose.cells.pivot/pivotfield/dispose/)() | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al reset delle risorse non gestite. |
| [FilterByDate](../../aspose.cells.pivot/pivotfield/filterbydate/)(PivotFilterType, DateTime, DateTime) | Filtra per valori di data del campo pivot di riga o colonna. |
| [FilterByLabel](../../aspose.cells.pivot/pivotfield/filterbylabel/)(PivotFilterType, string, string) | Filtra per didascalie del campo pivot di riga o colonna. |
| [FilterByValue](../../aspose.cells.pivot/pivotfield/filterbyvalue/)(int, PivotFilterType, double, double) | Filtra per valori del campo pivot dei dati. |
| [FilterTop10](../../aspose.cells.pivot/pivotfield/filtertop10/)(int, PivotFilterType, bool, int) | Filtra per valori del campo pivot dei dati. |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula/)() | (**Obsolete.**) Ottiene la stringa della formula del campo calcolato specificato. |
| [GetFilters](../../aspose.cells.pivot/pivotfield/getfilters/)() | Recupera tutti i filtri pivot applicati a questo campo pivot. |
| [GetFormula](../../aspose.cells.pivot/pivotfield/getformula/)() | Recupera la formula del campo calcolato. Funziona solo per il campo calcolato. |
| [GetMaxValue](../../aspose.cells.pivot/pivotfield/getmaxvalue/)() | Recupera il valore massimo di questo campo. |
| [GetMinValue](../../aspose.cells.pivot/pivotfield/getminvalue/)() | Recupera il valore massimo di questo campo. |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype/)(PivotFilterType) | Recupera il filtro pivot del campo pivot per tipo |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters/)() | (**Obsolete.**) Recupera i filtri pivot del campo pivot |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals/)(PivotFieldSubtotalType) | Indica se mostrare il subtotale specificato per questo campo pivot. |
| [Group](../../aspose.cells.pivot/pivotfield/group/#group)() | Raggruppa automaticamente il campo. |
| [Group](../../aspose.cells.pivot/pivotfield/group/#group_1)(PivotFieldGroupOptions) | Raggruppa il campo pivot con opzioni. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby)(CustomPiovtFieldGroupItem[], bool) | (**Obsolete.**) Raggruppa il campo in modo personalizzato. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_1)(DiscreteGroupItem[], bool) | (**Obsolete.**) Raggruppa il campo in modo personalizzato. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_7)(double, bool) | (**Obsolete.**) Raggruppa automaticamente il campo con intervallo |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_6)(PivotGroupByType[], double, bool) | (**Obsolete.**) Raggruppa automaticamente il campo con interno |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_4)(double, double, double, bool) | (**Obsolete.**) Raggruppa il file per numero. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_5)(DateTime, DateTime, PivotGroupByType[], double, bool) | (**Obsolete.**) Raggruppa il file per i tipi di gruppo data. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_2)(bool, double, bool, double, double, bool) | (**Obsolete.**) Raggruppa il file per numero. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_3)(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) | (**Obsolete.**) Raggruppa il file per i tipi di gruppo data. |
| [HideAllDetails](../../aspose.cells.pivot/pivotfield/hidealldetails/)() | Nasconde tutti i dettagli di ogni elemento pivot. |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail/)(bool) | (**Obsolete.**) Imposta se i dettagli di tutti i PivotItems in un campo pivot sono nascosti. Cioè comprimi/espandi questo campo. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem/#hideitem)(int, bool) | (**Obsolete.**) Imposta se lo specifico PivotItem in un campo dati è nascosto. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem/#hideitem_1)(string, bool) | (**Obsolete.**) Imposta se lo specifico PivotItem in un campo dati è nascosto. |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail/)(int, bool) | (**Obsolete.**) Imposta se il dettaglio dello specifico PivotItem in un campo pivot è nascosto. |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems/)() | (**Obsolete.**) Inizializza gli elementi pivot del campo pivot |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem/)(int) | (**Obsolete.**) Indica se lo specifico PivotItem è nascosto. |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail/)(int) | (**Obsolete.**) Indica se nascondere il dettaglio dello specifico PivotItem. |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals/)(PivotFieldSubtotalType, bool) | Imposta come subtotale il campo specificato. |
| [ShowAllDetails](../../aspose.cells.pivot/pivotfield/showalldetails/)() | Mostra tutti i dettagli di ogni elemento pivot. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/#showvaluesas_1)(PivotShowValuesAsType, int, int) | Imposta il calcolo \"Show Values As\" per questo campo pivot. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/#showvaluesas_2)(PivotShowValuesAsType, string, string) | Configura il calcolo \"Show Values As\" per questo campo dati. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/#showvaluesas)(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) | (**Obsolete.**) Mostra i valori del campo dati in un formato di visualizzazione diverso quando il calcolo ShowDataAs è in uso. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby)(SortOrder) | Ordina questo campo pivot. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_1)(SortOrder, int) | (**Obsolete.**) Ordina questo campo pivot. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_3)(SortOrder, int, string) | Ordina questo campo pivot. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_2)(SortOrder, int, PivotLineType, string) | (**Obsolete.**) Ordina questo campo pivot. |
| [Top10AutoShow](../../aspose.cells.pivot/pivotfield/top10autoshow/)(bool, bool, int, int) | Configura le impostazioni Top10 AutoShow per questo campo pivot. |
| [Ungroup](../../aspose.cells.pivot/pivotfield/ungroup/)() | Annulla il raggruppamento del campo pivot. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldDemo
    {
        public static void PivotFieldExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi alcuni dati al worksheet
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Aggiungi una tabella pivot al foglio di lavoro
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "year");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "amount");

            // Imposta lo stile della tabella pivot
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Accedi al campo di riga
            PivotField rowField = pivotTable.RowFields[0];

            // Imposta le proprietà del PivotField
            rowField.DisplayName = "Custom Display Name";
            rowField.IsAutoSubtotals = false;
            rowField.DragToColumn = true;
            rowField.DragToHide = true;
            rowField.DragToRow = true;
            rowField.DragToPage = true;
            rowField.DragToData = true;
            rowField.IsMultipleItemSelectionAllowed = true;
            rowField.IsRepeatItemLabels = true;
            rowField.IsIncludeNewItemsInFilter = true;
            rowField.IsInsertPageBreaksBetweenItems = true;
            rowField.ShowAllItems = true;
            rowField.NonAutoSortDefault = true;
            rowField.IsAutoSort = true;
            rowField.IsAscendSort = true;
            rowField.AutoSortField = -1;
            rowField.IsAutoShow = true;
            rowField.IsAscendShow = true;
            rowField.AutoShowCount = 5;
            rowField.AutoShowField = -1;
            rowField.Function = ConsolidationFunction.Sum;
            rowField.ShowValuesAs(PivotFieldDataDisplayFormat.PercentageOfTotal, 0, PivotItemPositionType.Next, 0);
            rowField.CurrentPageItem = 1;
            rowField.Number = 0;
            rowField.InsertBlankRow = true;
            rowField.ShowSubtotalAtTop = true;
            rowField.ShowInOutlineForm = true;
            rowField.NumberFormat = "0.00";
            rowField.ShowCompact = true;

            // Aggiorna e calcola i dati della tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotFieldExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


