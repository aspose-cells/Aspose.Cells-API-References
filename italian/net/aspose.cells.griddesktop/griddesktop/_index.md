---
title: "Classe GridDesktop"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.GridDesktop.GridDesktop class. La classe Aspose GridDesktop rappresenta un oggetto radice per creare un controllo GridDesktop. Per utilizzare questo controllo basta trascinarlo dalla casella degli strumenti su un form o su un usercontrol"
type: docs
url: /it/net/aspose.cells.griddesktop/griddesktop/
---
## GridDesktop class

La classe Aspose GridDesktop rappresenta un oggetto radice per creare un controllo GridDesktop. Per utilizzare questo controllo, basta trascinarlo dalla casella degli strumenti su un form o su un usercontrol.

```csharp
public class GridDesktop : UserControl
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridDesktop](griddesktop/)() | Classe Aspose GridDesktop |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells.griddesktop/griddesktop/activesheetindex/) { get; set; } | Ottiene o imposta l'indice del foglio selezionato. |
| [ActiveSheetNameFont](../../aspose.cells.griddesktop/griddesktop/activesheetnamefont/) { get; set; } | Ottiene o imposta il carattere visualizzato del foglio attivo nella barra dei fogli. |
| [AlwasysRecalculateAllFormulas](../../aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas/) { get; set; } | Ottiene o imposta un valore che indica se è necessario eseguire tutte le formule, come quando eseguiamo tutte le formule, quando si aggiorna il valore di una cella, e questa influisce su altre, e le altre influiscono su altre, sempre di più, causando la necessità di ricalcolare tutte le celle, proprio come l'effetto farfalla, richiede molte operazioni di stack, porta a prestazioni molto basse, come in CELLSNET-41921, questo problema contiene il file che può mostrare questo scenario; è meglio eseguire semplicemente tutte le formule, poiché quando si eseguono tutte le formule potremmo avere qualche ottimizzazione. |
| [BorderStyle](../../aspose.cells.griddesktop/griddesktop/borderstyle/) { get; set; } | Indica lo stile del bordo per il controllo. |
| [ColumnHeaderVisible](../../aspose.cells.griddesktop/griddesktop/columnheadervisible/) { get; set; } | Ottiene o imposta un valore che indica se l'intestazione della colonna è visibile. |
| [CommentDisplayingFont](../../aspose.cells.griddesktop/griddesktop/commentdisplayingfont/) { get; set; } | Ottiene o imposta il carattere di visualizzazione predefinito del testo del commento. |
| [ContextMenuManager](../../aspose.cells.griddesktop/griddesktop/contextmenumanager/) { get; } | Ottiene l'istanza di ContextMenuManager. |
| [DefaultCellFont](../../aspose.cells.griddesktop/griddesktop/defaultcellfont/) { get; set; } | Ottiene o imposta il carattere predefinito della cella |
| [DefaultCellFontColor](../../aspose.cells.griddesktop/griddesktop/defaultcellfontcolor/) { get; set; } | Ottiene o imposta il colore del carattere predefinito della cella. |
| [EnableClipboardCopyPaste](../../aspose.cells.griddesktop/griddesktop/enableclipboardcopypaste/) { get; set; } | Indica se copiare/incollare basandosi negli appunti, in modo da poter copiare/incollare con MS-EXCEL. Copia/incolla solo il valore della cella, non copia alcuna altra impostazione della cella come formato, stile del bordo e così via. Il valore predefinito è false. |
| [EnableCopyWithExtension](../../aspose.cells.griddesktop/griddesktop/enablecopywithextension/) { get; set; } | Ottiene o imposta un valore che indica se l'operazione di copia estenderà il numero di righe o colonne. |
| [EnableCopyWithLockedOption](../../aspose.cells.griddesktop/griddesktop/enablecopywithlockedoption/) { get; set; } | Ottiene o imposta un valore che indica se l'operazione di copia copierà il valore dell'attributo CellLocked dello stile di una cella. |
| [EnableUndo](../../aspose.cells.griddesktop/griddesktop/enableundo/) { get; set; } | Ottiene o imposta un valore che indica se la funzione Undo è abilitata. Il valore predefinito è false. |
| [GridMemorySetting](../../aspose.cells.griddesktop/griddesktop/gridmemorysetting/) { get; set; } | Ottiene o imposta l'opzione di memoria, il valore predefinito è GridMemorySetting.Normal |
| [IsHorizontalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/ishorizontalscrollbarvisible/) { get; set; } | Imposta lo stato di visibilità per la barra di scorrimento orizzontale. |
| [IsVerticalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/isverticalscrollbarvisible/) { get; set; } | Imposta lo stato di visibilità per la barra di scorrimento verticale. |
| [Names](../../aspose.cells.griddesktop/griddesktop/names/) { get; } | Ottiene la collezione di tutti gli oggetti Name nel foglio elettronico. |
| [PageRows](../../aspose.cells.griddesktop/griddesktop/pagerows/) { get; set; } | Imposta o ottiene la dimensione della riga per la paginazione. Il massimo di PageRows supportato è 100000, il massimo numero di pagina supportato è 5000. |
| [PasteType](../../aspose.cells.griddesktop/griddesktop/pastetype/) { get; set; } | Indica il tipo di incolla da utilizzare durante l'azione di incolla, disponibile solo quando EnableClipboardCopyPaste è false. Il valore predefinito è GridPasteType.Default; |
| [R1C1](../../aspose.cells.griddesktop/griddesktop/r1c1/) { get; set; } | Ottiene o imposta un valore che indica se il controllo utilizza lo stile di riferimento R1C1. |
| [RecalculateFormulas](../../aspose.cells.griddesktop/griddesktop/recalculateformulas/) { get; set; } | Ottiene o imposta un valore che indica se ricalcolare tutte le formule delle celle quando il valore di una cella cambia. Il valore predefinito è true. |
| [RowHeaderVisible](../../aspose.cells.griddesktop/griddesktop/rowheadervisible/) { get; set; } | Ottiene o imposta un valore che indica se l'intestazione di riga è visibile. |
| [SheetNameFont](../../aspose.cells.griddesktop/griddesktop/sheetnamefont/) { get; set; } | Ottiene o imposta il carattere di visualizzazione predefinito della barra del foglio. |
| [SheetsBarVisible](../../aspose.cells.griddesktop/griddesktop/sheetsbarvisible/) { get; set; } | Ottiene o imposta un valore che indica se la barra del foglio è visibile. |
| [SheetTabWidth](../../aspose.cells.griddesktop/griddesktop/sheettabwidth/) { get; set; } | Imposta / ottiene la larghezza della scheda del foglio. |
| [ShowContextMenu](../../aspose.cells.griddesktop/griddesktop/showcontextmenu/) { get; set; } | Ottiene o imposta un valore che indica se il controllo può mostrare il menu contestuale. |
| [ShowFormulaWarning](../../aspose.cells.griddesktop/griddesktop/showformulawarning/) { get; set; } | Imposta / ottiene se mostrare il messaggio di errore o avviso per l'impostazione del valore della formula della cella, il valore predefinito è true. |
| [ShowNumberStoredAsTextSymbol](../../aspose.cells.griddesktop/griddesktop/shownumberstoredastextsymbol/) { get; set; } | Imposta / ottiene se mostrare il simbolo a triangolo per la cella che contiene una stringa numerica ma è memorizzata come formato testo |
| [ShowStatus](../../aspose.cells.griddesktop/griddesktop/showstatus/) { get; set; } | Ottiene o imposta un valore che indica se mostrare lo stato di calcolo. Il valore predefinito è true. |
| [UndoManager](../../aspose.cells.griddesktop/griddesktop/undomanager/) { get; } | Ottiene l'istanza di UndoManager. |
| [Worksheets](../../aspose.cells.griddesktop/griddesktop/worksheets/) { get; } | Ottiene i fogli di lavoro. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Clear](../../aspose.cells.griddesktop/griddesktop/clear/)() | Cancella il controllo GridDesktop. |
| [Copy](../../aspose.cells.griddesktop/griddesktop/copy/)() | Copia il contenuto della cella focalizzata negli appunti. |
| [Cut](../../aspose.cells.griddesktop/griddesktop/cut/)() | Taglia il contenuto della cella focalizzata negli appunti. |
| [DoSplit](../../aspose.cells.griddesktop/griddesktop/dosplit/)() | Imposta la visualizzazione divisa. |
| [EndFormatPainter](../../aspose.cells.griddesktop/griddesktop/endformatpainter/)() | Notifica a GridDesktop di terminare FormatPainter. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile)(Stream) | Esporta in un flusso di file Excel, includendo flusso di I/O disco o flusso di memoria. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_2)(string) | Esporta in un file Excel. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_1)(Stream, FileFormatType) | Esporta in un flusso di file Excel, includendo flusso di I/O disco o flusso di memoria. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_3)(string, FileFormatType) | Esporta in un file Excel. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile)(Stream, GridPdfSaveOptions) | Esporta in un flusso di file PDF, includendo flusso di I/O su disco o flusso di memoria. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile_1)(string, GridPdfSaveOptions) | Esporta in un flusso di file PDF, includendo flusso di I/O su disco o flusso di memoria. |
| [GetActiveWorksheet](../../aspose.cells.griddesktop/griddesktop/getactiveworksheet/)() | Ottiene il foglio di lavoro attivo corrente. |
| [getHScrollBar](../../aspose.cells.griddesktop/griddesktop/gethscrollbar/)() | restituisce la barra di scorrimento orizzontale |
| [getVScrollBar](../../aspose.cells.griddesktop/griddesktop/getvscrollbar/)() | restituisce la barra di scorrimento verticale |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile)(Stream) | Importa da un flusso di file Excel, includendo flusso da disco o flusso di memoria. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_3)(string) | Importa da un file Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_1)(Stream, bool) | Importa da un flusso di file Excel, includendo flusso da disco o flusso di memoria. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_4)(string, bool) | Importa da un file Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_5)(string, int) | Importa un foglio di lavoro da un file Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_2)(Stream, string, string, bool, bool) | Importa da un file Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_6)(string, string, string, bool, bool) | Importa da un file Excel. |
| [Invalidate](../../aspose.cells.griddesktop/griddesktop/invalidate/#invalidate)() | Sovrascrivi invalidate. |
| [OpenFindReplaceDialog](../../aspose.cells.griddesktop/griddesktop/openfindreplacedialog/)(bool) | Apre la finestra di dialogo FindReplace per trovare o sostituire celle. |
| [Paste](../../aspose.cells.griddesktop/griddesktop/paste/)() | Incolla il contenuto degli appunti nella cella focalizzata. |
| [RefreshControl](../../aspose.cells.griddesktop/griddesktop/refreshcontrol/)() | Aggiorna il controllo GridDesktop. |
| [RunAllFormulas](../../aspose.cells.griddesktop/griddesktop/runallformulas/)() | Esegue tutte le formule delle celle. |
| [SetAllScrollBarsVisible](../../aspose.cells.griddesktop/griddesktop/setallscrollbarsvisible/)() | Imposta tutte le barre di scorrimento visibili. |
| [SetCustomResourceManager](../../aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/)(ResourceManager) | Imposta un gestore di risorse personalizzato per implementare la localizzazione definita dall'utente |
| [ShowStyleDialog](../../aspose.cells.griddesktop/griddesktop/showstyledialog/)() | Apre una finestra di dialogo stile per impostare lo stile delle celle, il carattere, i colori ecc. |
| [StartFormatPainter](../../aspose.cells.griddesktop/griddesktop/startformatpainter/)(bool) | Notifica GridDesktop di avviare FormatPainter. |
| [UnDoSplit](../../aspose.cells.griddesktop/griddesktop/undosplit/)() | Disattiva la visualizzazione Split. |
| static [GetVersion](../../aspose.cells.griddesktop/griddesktop/getversion/)() | Ottiene la versione di rilascio. |

## Campi

| Nome | Descrizione |
| --- | --- |
| [LoadDataFilter](../../aspose.cells.griddesktop/griddesktop/loaddatafilter/) | le opzioni per filtrare i dati durante il caricamento della cartella di lavoro dal modello. |
| [ShowImportMessage](../../aspose.cells.griddesktop/griddesktop/showimportmessage/) | se mostrare la finestra di messaggio quando il caricamento del file fallisce, il valore predefinito è true |

## Eventi

| Nome | Descrizione |
| --- | --- |
| event [AfterDeleteColumns](../../aspose.cells.griddesktop/griddesktop/afterdeletecolumns/) | Si verifica dopo che la colonna è stata eliminata. |
| event [AfterDeleteRows](../../aspose.cells.griddesktop/griddesktop/afterdeleterows/) | Si verifica dopo che la riga è stata eliminata. |
| event [AfterInsertColumns](../../aspose.cells.griddesktop/griddesktop/afterinsertcolumns/) | Si verifica dopo l'inserimento di una nuova colonna. |
| event [AfterInsertRows](../../aspose.cells.griddesktop/griddesktop/afterinsertrows/) | Si verifica dopo l'inserimento di una nuova riga. |
| event [BeforeCalculate](../../aspose.cells.griddesktop/griddesktop/beforecalculate/) | Si verifica prima del calcolo della formula nella cartella di lavoro. |
| event [BeforeLoadFile](../../aspose.cells.griddesktop/griddesktop/beforeloadfile/) | Si verifica prima che la cartella di lavoro venga caricata dal file. |
| event [CellButtonClick](../../aspose.cells.griddesktop/griddesktop/cellbuttonclick/) | Si verifica quando il pulsante della cella viene cliccato. |
| event [CellCheckedChanged](../../aspose.cells.griddesktop/griddesktop/cellcheckedchanged/) | Si verifica quando la proprietà Checked della casella di controllo della cella viene modificata. |
| event [CellClick](../../aspose.cells.griddesktop/griddesktop/cellclick/) | Si verifica quando la cella della griglia viene cliccata. |
| event [CellComboBoxCopy](../../aspose.cells.griddesktop/griddesktop/cellcomboboxcopy/) | Si verifica quando un ComboBox di una cella della griglia viene copiato. |
| event [CellDataChanged](../../aspose.cells.griddesktop/griddesktop/celldatachanged/) | Si verifica quando la proprietà dati della cella della griglia viene modificata. |
| event [CellDoubleClick](../../aspose.cells.griddesktop/griddesktop/celldoubleclick/) | Si verifica quando la cella della griglia viene doppio cliccata. |
| event [CellFormatChanged](../../aspose.cells.griddesktop/griddesktop/cellformatchanged/) | Si verifica quando il formato della cella viene modificato tramite la finestra di dialogo Formatta celle. |
| event [CellKeyPressed](../../aspose.cells.griddesktop/griddesktop/cellkeypressed/) | Si verifica quando viene premuto un tasto mentre una cella ha il focus. |
| event [CellSelectedIndexChanged](../../aspose.cells.griddesktop/griddesktop/cellselectedindexchanged/) | Si verifica quando la proprietà SelectedIndex del combobox della cella è cambiata. |
| event [CellTextBoxChanging](../../aspose.cells.griddesktop/griddesktop/celltextboxchanging/) | Si verifica quando si digitano caratteri in una cella della griglia. |
| event [CellValidationFailed](../../aspose.cells.griddesktop/griddesktop/cellvalidationfailed/) | Si verifica quando la convalida di una cella della griglia fallisce. |
| event [ColumnHeaderClick](../../aspose.cells.griddesktop/griddesktop/columnheaderclick/) | Si verifica quando l'intestazione della colonna viene cliccata. |
| event [ColumnHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/columnheaderdoubleclick/) | Si verifica quando l'intestazione della colonna viene doppio cliccata. |
| event [CommentDataChanged](../../aspose.cells.griddesktop/griddesktop/commentdatachanged/) | Si verifica quando i dati del commento sono cambiati. |
| event [FailLoadFile](../../aspose.cells.griddesktop/griddesktop/failloadfile/) |  |
| event [FinishCalculate](../../aspose.cells.griddesktop/griddesktop/finishcalculate/) | Si verifica dopo il calcolo della formula nella cartella di lavoro. |
| event [FinishLoadFile](../../aspose.cells.griddesktop/griddesktop/finishloadfile/) | Si verifica quando la cartella di lavoro viene caricata. |
| event [FocusedCellChanged](../../aspose.cells.griddesktop/griddesktop/focusedcellchanged/) | Si verifica quando la cella con focus viene cambiata. |
| event [PictureClick](../../aspose.cells.griddesktop/griddesktop/pictureclick/) | Si verifica quando la forma viene cliccata. |
| event [RowColumnHiddenChanged](../../aspose.cells.griddesktop/griddesktop/rowcolumnhiddenchanged/) | Si verifica quando lo stato di nascondi riga/colonna è cambiato. |
| event [RowFilteredEvent](../../aspose.cells.griddesktop/griddesktop/rowfilteredevent/) | Si verifica dopo la selezione di un elemento del filtro di riga. |
| event [RowHeaderClick](../../aspose.cells.griddesktop/griddesktop/rowheaderclick/) | Si verifica quando l'intestazione della riga viene cliccata. |
| event [RowHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/rowheaderdoubleclick/) | Si verifica quando l'intestazione della riga viene doppio cliccata. |
| event [SelectedCellRangeChanged](../../aspose.cells.griddesktop/griddesktop/selectedcellrangechanged/) | Si verifica quando l'intervallo di celle selezionato viene cambiato. |
| event [SelectedSheetIndexChanged](../../aspose.cells.griddesktop/griddesktop/selectedsheetindexchanged/) | Si verifica quando la proprietà SelectedSheetIndex è cambiata. |
| event [ShapeClick](../../aspose.cells.griddesktop/griddesktop/shapeclick/) | Si verifica quando la forma viene cliccata. |

### Osservazioni

Fare riferimento al documento .NET SDK per ulteriori informazioni su System.Windows.Forms.UserControl.

### Esempi

```csharp
[C#]
gridDesktop1.Worksheets[0].Cells[0, 0].Value = "2";
gridDesktop1.Worksheets[0].Cells[1, 0].Value = "3";
gridDesktop1.Worksheets[0].Cells[2, 1].Value = "=a1*a2";
gridDesktop1.RunAllFormulas();
gridDesktop1.Invalidate();

[Visual Basic]
gridDesktop1.Worksheets(0).Cells(0, 0).Value = "2"
gridDesktop1.Worksheets(0).Cells(1, 0).Value = "3"
gridDesktop1.Worksheets(0).Cells(2, 1).Value = "=a1*a2"
gridDesktop1.RunAllFormulas()
gridDesktop1.Invalidate()

```

### Vedi anche

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


