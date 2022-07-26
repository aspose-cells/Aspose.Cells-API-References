---
title: PivotField
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta un campo in un report di tabella pivot.
type: docs
weight: 4530
url: /it/net/aspose.cells.pivot/pivotfield/
---
## PivotField class

Rappresenta un campo in un report di tabella pivot.

```csharp
public class PivotField
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoShowCount](../../aspose.cells.pivot/pivotfield/autoshowcount) { get; set; } | Rappresenta il numero di elementi in alto o in basso visualizzati automaticamente nel campo Tabella pivot specificato. |
| [AutoShowField](../../aspose.cells.pivot/pivotfield/autoshowfield) { get; set; } | Rappresenta l'indice del campo di visualizzazione automatica. -1 significa PivotField stesso. Dovrebbe essere l'indice dei campi di dati. |
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield) { get; set; } | Rappresenta l'indice del campo di ordinamento automatico. -1 significa PivotField stesso, altri indica la posizione dei campi di dati. |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotfield/basefieldindex) { get; set; } | Rappresenta il campo base per un calcolo personalizzato. |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex) { get; set; } | Rappresenta l'indice PivotField nei PivotField di base. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotfield/baseitemindex) { get; set; } | Rappresenta l'elemento nel campo di base per un calcolo personalizzato. Valido solo per i campi di dati. |
| [BaseItemPosition](../../aspose.cells.pivot/pivotfield/baseitemposition) { get; set; } | Rappresenta l'elemento nel campo di base per un calcolo personalizzato. Valido solo per i campi di dati. Poiché PivotItemPosition.Custom è solo per la lettura, se è necessario impostare PivotItemPosition.Custom, impostare l'attributo PivotField.BaseItemIndex. |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem) { get; set; } | Rappresenta l'elemento della pagina corrente visualizzato per il campo della pagina (valido solo per i campi della pagina). |
| [DataDisplayFormat](../../aspose.cells.pivot/pivotfield/datadisplayformat) { get; set; } | Rappresenta come visualizzare i valori contenuti in un campo dati. |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname) { get; set; } | Rappresenta il nome visualizzato del campo pivot. |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn) { get; set; } | Indica se il campo specificato può essere trascinato nella posizione della colonna. Il valore predefinito è true. |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata) { get; set; } | Indica se il campo specificato può essere trascinato nella posizione dei dati. Il valore predefinito è true. |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide) { get; set; } | Indica se il campo specificato può essere trascinato nella posizione nascosta. Il valore predefinito è true. |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage) { get; set; } | Indica se il campo specificato può essere trascinato nella posizione della pagina. Il valore predefinito è true. |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow) { get; set; } | Indica se il campo specificato può essere trascinato nella posizione della riga. Il valore predefinito è true. |
| [Function](../../aspose.cells.pivot/pivotfield/function) { get; set; } | Rappresenta la funzione utilizzata per riepilogare il campo dati della tabella pivot. |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow) { get; set; } | Indica se inserire una riga vuota dopo ogni elemento. |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow) { get; set; } | Indica se il campo della tabella pivot specificato viene visualizzato automaticamente in modo crescente. |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort) { get; set; } | Indica se il campo della tabella pivot specificato viene ordinato automaticamente in modo crescente. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow) { get; set; } | Indica se il campo tabella pivot specificato viene visualizzato automaticamente, valido solo per excel 2003. |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort) { get; set; } | Indica se il campo della tabella pivot specificato viene ordinato automaticamente. |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals) { get; set; } | Indica se il campo specificato mostra i totali parziali automatici. L'impostazione predefinita è true. |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield) { get; } | Indica se il campo tabella pivot specificato è un campo calcolato. |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter) { get; set; } | indica se il campo può includere nuovi elementi nel filtro manuale Il valore predefinito è false. |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems) { get; set; } | indica se il campo può inserire interruzioni di pagina tra gli elementi inserire un'interruzione di pagina dopo ogni elemento Il valore predefinito è false. |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed) { get; set; } | indica se il campo può avere più elementi selezionati nel campo della pagina Il valore predefinito è false. |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels) { get; set; } | indica se il campo può ripetere gli elementi labels Il valore predefinito è false. |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount) { get; } | Ottiene il conteggio degli elementi di base di questo campo pivot. |
| [Items](../../aspose.cells.pivot/pivotfield/items) { get; } | Ottieni tutti gli elementi di base; |
| [Name](../../aspose.cells.pivot/pivotfield/name) { get; } | Rappresenta il nome del campo pivot. |
| [Number](../../aspose.cells.pivot/pivotfield/number) { get; set; } | Rappresenta il formato di visualizzazione integrato di numeri e date. |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat) { get; set; } | Rappresenta il formato di visualizzazione personalizzato di numeri e date. |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems) { get; } | Ottieni gli elementi di base originali; |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems) { get; } | Ottiene gli elementi pivot del campo pivot |
| [Position](../../aspose.cells.pivot/pivotfield/position) { get; } | Rappresenta l'indice PivotField nei PivotField. |
| [Range](../../aspose.cells.pivot/pivotfield/range) { get; } | Ottiene l'intervallo di gruppo del campo pivot |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems) { get; set; } | Indica se vengono visualizzati tutti gli elementi nel rapporto tabella pivot, anche se non contengono dati di riepilogo. mostra elementi senza dati Il valore predefinito è false. |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact) { get; set; } | Indica se visualizzare le etichette dal campo successivo nella stessa colonna nella vista tabella pivot |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform) { get; set; } | Indica se il layout di questo campo sotto forma di struttura nella vista tabella pivot |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop) { get; set; } | quando ShowInOutlineForm è true, quindi mostra i totali parziali nella parte superiore dell'elenco di elementi anziché nella parte inferiore |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem)(string, string) | Aggiungi un elemento calcolato al campo pivot. |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula)() | Ottieni la stringa della formula del campo calcolato specificato . |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype)(PivotFilterType) | Ottiene il filtro pivot del campo pivot per tipo |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters)() | Ottiene i filtri pivot del campo pivot |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals)(PivotFieldSubtotalType) | Ottiene se il campo specificato mostra i totali parziali. |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail)(bool) | Imposta se i PivotItems in un campo pivot sono dettagli nascosti. Ovvero comprimi/espandi questo campo. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem)(int, bool) | Imposta se l'elemento pivot specifico in un campo dati è nascosto. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem_1)(string, bool) | Imposta se l'elemento pivot specifico in un campo dati è nascosto. |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail)(int, bool) | Imposta se l'elemento pivot specifico in un campo pivot è nascosto nei dettagli. |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems)() | Inizializza gli elementi pivot del campo pivot |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem)(int) | Indica se il PivotItem specifico è nascosto. |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail)(int) | Indica se il PivotItem specifico è un dettaglio nascosto. |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals)(PivotFieldSubtotalType, bool) | Imposta se il campo specificato mostra i totali parziali. |

### Esempi

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
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

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//Modifica gli attributi di PivotField
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

pivot.RefreshData();
pivot.CalculateData();

//fai i tuoi affari

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Guarda anche

* spazio dei nomi [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
