---
title: GridWorksheet
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula loggetto che rappresenta un singolo foglio di lavoro.
type: docs
weight: 570
url: /it/net/aspose.cells.gridweb.data/gridworksheet/
---
## GridWorksheet class

Incapsula l'oggetto che rappresenta un singolo foglio di lavoro.

```csharp
public class GridWorksheet : Control, ISerializable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb.data/gridworksheet/activecell) { get; set; } |  |
| [BackgroundImage](../../aspose.cells.gridweb.data/gridworksheet/backgroundimage) { get; set; } | Ottiene e imposta l'immagine di sfondo del foglio di lavoro. |
| [BindColumns](../../aspose.cells.gridweb.data/gridworksheet/bindcolumns) { get; } | Collezione colonne Bind. |
| [BindingSource](../../aspose.cells.gridweb.data/gridworksheet/bindingsource) { get; } | L'oggetto origine dati effettivamente vincolante in fase di esecuzione. È un oggetto DataView quando la proprietà DataSource è un oggetto DataSet, DataTable o DataView. |
| [BindStartColumn](../../aspose.cells.gridweb.data/gridworksheet/bindstartcolumn) { get; set; } | In modalità di associazione dati, BindStartRow e BindStartColumn indicano la posizione della griglia per associare l'origine dati. |
| [BindStartRow](../../aspose.cells.gridweb.data/gridworksheet/bindstartrow) { get; set; } | In modalità di associazione dati, BindStartRow e BindStartColumn indicano la posizione della griglia per associare l'origine dati. |
| [Cells](../../aspose.cells.gridweb.data/gridworksheet/cells) { get; } |  |
| [CodeName](../../aspose.cells.gridweb.data/gridworksheet/codename) { get; } | Rappresenta il nome del codice del foglio di lavoro. |
| [Comments](../../aspose.cells.gridweb.data/gridworksheet/comments) { get; } |  |
| [CurrentBindRows](../../aspose.cells.gridweb.data/gridworksheet/currentbindrows) { get; set; } | Ottiene il numero di righe di associazione in modalità di associazione dati. |
| [DataMember](../../aspose.cells.gridweb.data/gridworksheet/datamember) { get; set; } | Ottiene o imposta DataMember da DataSource a più membri. Generalmente rappresenta un oggetto DataTable di un DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/gridworksheet/datasource) { get; set; } | Ottiene o imposta DataSource. Generalmente è un oggetto DataSet. |
| [DisplayRightToLeft](../../aspose.cells.gridweb.data/gridworksheet/displayrighttoleft) { get; set; } |  |
| [DisplayZeros](../../aspose.cells.gridweb.data/gridworksheet/displayzeros) { get; set; } | Vero se vengono visualizzati valori zero. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/gridworksheet/enablecreatebindcolumnheader) { get; set; } | In modalità di associazione dati, indica se creare didascalie di intestazione di colonna bind nel foglio. |
| [FirstVisibleColumn](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblecolumn) { get; set; } |  |
| [FirstVisibleRow](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblerow) { get; set; } |  |
| [GridActiveCell](../../aspose.cells.gridweb.data/gridworksheet/gridactivecell) { get; set; } |  |
| [Hyperlinks](../../aspose.cells.gridweb.data/gridworksheet/hyperlinks) { get; } | Ottiene ilHyperlinkCollection raccolta. |
| [Index](../../aspose.cells.gridweb.data/gridworksheet/index) { get; } |  |
| [IsGridlinesVisible](../../aspose.cells.gridweb.data/gridworksheet/isgridlinesvisible) { get; set; } | Ottiene o imposta un valore che indica se le linee della griglia sono visibili. L'impostazione predefinita è true. |
| [IsSummaryRowBelow](../../aspose.cells.gridweb.data/gridworksheet/issummaryrowbelow) { get; set; } | Indica se la riga di riepilogo verrà posizionata al di sotto delle righe di dettaglio nella struttura. |
| [Name](../../aspose.cells.gridweb.data/gridworksheet/name) { get; set; } | Ottiene o imposta il nome del foglio di lavoro. |
| [OutlineShown](../../aspose.cells.gridweb.data/gridworksheet/outlineshown) { get; set; } | Indica se mostrare il contorno. |
| [Pictures](../../aspose.cells.gridweb.data/gridworksheet/pictures) { get; } | Ottiene a[`Pictures`](./pictures) raccolta. |
| [PivotTables](../../aspose.cells.gridweb.data/gridworksheet/pivottables) { get; } | Ottiene le tabelle pivot nel foglio di lavoro. |
| [Selected](../../aspose.cells.gridweb.data/gridworksheet/selected) { get; set; } | Indica se questo foglio di lavoro è selezionato all'apertura della cartella di lavoro. |
| [Shapes](../../aspose.cells.gridweb.data/gridworksheet/shapes) { get; } | Ottiene a[`Pictures`](./pictures) raccolta. |
| [StandardHeight](../../aspose.cells.gridweb.data/gridworksheet/standardheight) { get; set; } | Ottiene o imposta l'altezza della riga predefinita in questo foglio di lavoro, in unità di punti. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridworksheet/standardheightpixels) { get; set; } | Ottiene o imposta l'altezza della riga predefinita in questo foglio di lavoro, in unità di pixel. |
| [TabColor](../../aspose.cells.gridweb.data/gridworksheet/tabcolor) { get; set; } | Rappresenta il colore della scheda del foglio di lavoro. |
| [Validations](../../aspose.cells.gridweb.data/gridworksheet/validations) { get; } | Ottiene la raccolta delle impostazioni di convalida dei dati nel foglio di lavoro. |
| override [Visible](../../aspose.cells.gridweb.data/gridworksheet/visible) { get; set; } | Indica se il nome di questo foglio è mostrato nelle schede del foglio del controllo. |
| [Workbook](../../aspose.cells.gridweb.data/gridworksheet/workbook) { get; } |  |
| [Zoom](../../aspose.cells.gridweb.data/gridworksheet/zoom) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/addautofilter)(int, int, int) | Imposta l'intervallo a cui si applica il filtro automatico specificato. |
| [AddCustomFilter](../../aspose.cells.gridweb.data/gridworksheet/addcustomfilter)(int, string) | Aggiungi un filtro personalizzato per la riga specificata. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn#autofitcolumn)(int) | Adatta automaticamente la larghezza della colonna. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn#autofitcolumn_1)(int, int, int) | Adatta automaticamente la larghezza della colonna. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow#autofitrow)(int) | Adatta automaticamente l'altezza della riga. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow#autofitrow_1)(int, int, int) | Adatta automaticamente l'altezza della riga. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow#autofitrow_2)(int, int, int, int) | Adatta automaticamente l'altezza della riga in un intervallo di rettangoli. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows#autofitrows)() | Adatta automaticamente tutte le righe in questo foglio di lavoro. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows#autofitrows_1)(bool) | Adatta automaticamente tutte le righe in questo foglio di lavoro. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows#autofitrows_2)(int, int) | Adatta automaticamente l'altezza della riga in un intervallo. |
| [CalculateFormula](../../aspose.cells.gridweb.data/gridworksheet/calculateformula)(string) | Calcola una formula. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/cancelnewbindrow)() | Annulla ed elimina la nuova riga di collegamento aggiunta. |
| [ClearComments](../../aspose.cells.gridweb.data/gridworksheet/clearcomments)() | Cancella tutti i commenti nel foglio di calcolo del designer. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/commitnewbindrow)() | Conferma la nuova riga di collegamento aggiunta e la aggiunge all'origine dati. |
| [Copy](../../aspose.cells.gridweb.data/gridworksheet/copy)(GridWorksheet) | Copia contenuti e formati da un altro foglio di lavoro. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/gridworksheet/createautogenratedcolumns)() | Dopo aver impostato un'origine dati per il foglio di lavoro, chiama questo metodo per generare automaticamente le colonne di collegamento. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/createnewbindrow)() | Crea una nuova riga di collegamento e si collega all'origine dati. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal#createsubtotal)(int, int, int, SubtotalFunction, int[]) | Crea il totale parziale nel foglio. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal#createsubtotal_1)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Crea il totale parziale nel foglio. |
| override [DataBind](../../aspose.cells.gridweb.data/gridworksheet/databind)() | Associa il foglio a DataSource. |
| [DataSourceControlUpdate](../../aspose.cells.gridweb.data/gridworksheet/datasourcecontrolupdate)(AccessDataSource) | Associa il foglio a DataSource. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/gridworksheet/deletebindrow)(int) | Elimina una riga di collegamento. |
| [FilterString](../../aspose.cells.gridweb.data/gridworksheet/filterstring)(int, string) | Imposta il filtro per la colonna. Si noti che chiameremo AddAutoFilter prima di chiamare filterString La stringa dei criteri del filtro. avviso usiamo virgola-&gt;"," come carattere diviso, quindi il valore della cella che vuoi filtrare non deve contenere con virgola filterString(10,"123,456") significa che la colonna 10 deve contenere 123 o 456, filterString(10,"123" ) significa che la colonna 10 deve contenere 123 valore diviso con virgola, es. 123.456.789 o abc |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes#freezepanes_1)(string, int, int) | Blocca i riquadri nella cella specificata nel foglio di lavoro. |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes#freezepanes)(int, int, int, int) | Blocca i riquadri nella cella specificata nel foglio di lavoro. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/getcolumncaption)(int) | Ottiene la didascalia della colonna. Se la didascalia non è impostata, restituisce una stringa vuota. |
| [GetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getcolumnheadertooltip)(int) | Ottiene il testo della descrizione comando dell'intestazione della colonna. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/getcolumnreadonly)(int) | Ottiene se una colonna è di sola lettura. questo è specificamente il metodo esteso di GridWeb, non manterrà e non avrà effetto nel file excel effettivo |
| [GetFreezedPanes](../../aspose.cells.gridweb.data/gridworksheet/getfreezedpanes)(out int, out int, out int, out int) | Ottiene i riquadri di blocco. |
| [GetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/getisreadonly)(int, int) | Ottiene se la cella è di sola lettura. Questo è un attributo esteso di GridWeb, non verrà mantenuto nel file excel effettivo |
| [GetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/getrowcaption)(int) | Ottiene la didascalia della riga. Se la didascalia non è impostata, restituisce una stringa vuota. |
| [GetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getrowheadertooltip)(int) | Ottiene il testo della descrizione comando dell'intestazione di riga. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/getrowreadonly)(int) | Ottiene se una riga è di sola lettura. questo è specificamente il metodo esteso di GridWeb, non manterrà e non avrà effetto nel file excel effettivo |
| [GroupRows](../../aspose.cells.gridweb.data/gridworksheet/grouprows)(int, int, bool) | Raggruppa righe. |
| [IsProtected](../../aspose.cells.gridweb.data/gridworksheet/isprotected)() | Indica se il foglio di lavoro è protetto. |
| [MoveTo](../../aspose.cells.gridweb.data/gridworksheet/moveto)(int) | Sposta il foglio in un'altra posizione nel foglio di calcolo. |
| [RefreshFilter](../../aspose.cells.gridweb.data/gridworksheet/refreshfilter)() | Aggiorna i filtri automatici per nascondere o mostrare le righe. |
| [RemoveAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/removeautofilter)() | Rimuovi il filtro automatico del foglio di lavoro. |
| [RemoveSubtotal](../../aspose.cells.gridweb.data/gridworksheet/removesubtotal)() | Rimuove il totale parziale creato dal metodo CreateSubtotal nel foglio. |
| [ResetFilter](../../aspose.cells.gridweb.data/gridworksheet/resetfilter)(int) | L'offset intero del campo su cui si desidera applicare, in base alla prima colonna del filtro (a sinistra dell'elenco; il campo più a sinistra è il campo 0). |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/gridworksheet/setallcellseditable)() | Rende modificabili tutte le celle. Questo è l'attributo esteso |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setallcellsreadonly)() | Rende tutte le celle di sola lettura. Questo è un attributo esteso nota che questo attributo non può essere mantenuto nella cella effettiva, se vuoi mantenere la protezione usa setProtect |
| [SetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/setcolumncaption)(int, string) | Imposta la didascalia per la colonna. Si prega di notare che questo è un attributo di estensione e non può essere conservato nel file excel |
| [SetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setcolumnheadertooltip)(int, string) | Imposta il testo della descrizione comando dell'intestazione della colonna. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/setcolumnreadonly)(int, bool) | Imposta una colonna in sola lettura in modo che l'utente non possa eliminarla dal lato client. questo è un metodo esteso di GridWeb in particolare, non manterrà e non avrà effetto nel file excel effettivo |
| [SetEditableRange](../../aspose.cells.gridweb.data/gridworksheet/seteditablerange)(int, int, int, int) | Rende modificabile un intervallo di celle. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Rendi tutte le celle di sola lettura chiamando il metodo SetAllCellsReadonly. quindi chiama questo metodo per specificare l'intervallo di celle che devono essere modificabili |
| [SetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setisreadonly)(int, int, bool) | Imposta se la cella è di sola lettura. Questo è un attributo esteso di GridWeb, non verrà mantenuto nel file excel effettivo |
| [SetProtect](../../aspose.cells.gridweb.data/gridworksheet/setprotect)() | Protegge il foglio di lavoro. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/gridworksheet/setreadonlyrange)(int, int, int, int) | Rende un intervallo di celle di sola lettura. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Per prima cosa rendi modificabili tutte le celle chiamando il metodo SetAllCellsEditable. quindi chiama questo metodo per specificare l'intervallo di celle che devono essere di sola lettura |
| [SetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/setrowcaption)(int, string) | Imposta la didascalia per la riga. |
| [SetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setrowheadertooltip)(int, string) | Imposta il testo della descrizione comando dell'intestazione di riga. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/setrowreadonly)(int, bool) | Imposta una riga in sola lettura in modo che l'utente non possa eliminarla dal lato client. questo è un metodo esteso di GridWeb in particolare, non manterrà e non avrà effetto nel file excel effettivo |
| [UnFreezePanes](../../aspose.cells.gridweb.data/gridworksheet/unfreezepanes)() | Sblocca i riquadri nel foglio di lavoro. |
| [UnGroupRows](../../aspose.cells.gridweb.data/gridworksheet/ungrouprows)(int, int) | Separa le righe. |
| [UnProtect](../../aspose.cells.gridweb.data/gridworksheet/unprotect)() | foglio di lavoro non protegge. |

### Guarda anche

* spazio dei nomi [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* assemblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
