---
title: "Class GridWorksheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.GridWeb.Data.GridWorksheet class. Incapsula l'oggetto che rappresenta un singolo foglio di lavoro"
type: docs
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
| [ActiveCell](../../aspose.cells.gridweb.data/gridworksheet/activecell/) { get; set; } | Ottiene o imposta la cella attiva nel foglio di lavoro. |
| [BackgroundImage](../../aspose.cells.gridweb.data/gridworksheet/backgroundimage/) { get; set; } | Ottiene e imposta l'immagine di sfondo del foglio di lavoro. |
| [BindColumns](../../aspose.cells.gridweb.data/gridworksheet/bindcolumns/) { get; } | Associa la raccolta di colonne. |
| [BindingSource](../../aspose.cells.gridweb.data/gridworksheet/bindingsource/) { get; } | L'oggetto datasource effettivamente associato a runtime. È un oggetto DataView quando la proprietà DataSource è un oggetto DataSet, DataTable o DataView. |
| [BindStartColumn](../../aspose.cells.gridweb.data/gridworksheet/bindstartcolumn/) { get; set; } | In modalità data-binding, BindStartRow e BindStartColumn indicano la posizione della griglia da associare al datasource. |
| [BindStartRow](../../aspose.cells.gridweb.data/gridworksheet/bindstartrow/) { get; set; } | In modalità data-binding, BindStartRow e BindStartColumn indicano la posizione della griglia da associare al datasource. |
| [Cells](../../aspose.cells.gridweb.data/gridworksheet/cells/) { get; } | Ottiene la raccolta [`GridCell`](../gridcell/) . |
| [CodeName](../../aspose.cells.gridweb.data/gridworksheet/codename/) { get; } | Rappresenta il nome codice del foglio di lavoro. |
| [Comments](../../aspose.cells.gridweb.data/gridworksheet/comments/) { get; } | Ottiene la collezione [`GridComment`](../gridcomment/). |
| [CurrentBindRows](../../aspose.cells.gridweb.data/gridworksheet/currentbindrows/) { get; set; } | Ottiene il numero di righe di binding in modalità data-binding. |
| [DataMember](../../aspose.cells.gridweb.data/gridworksheet/datamember/) { get; set; } | Ottiene o imposta il DataMember dal DataSource multivalore. Generalmente rappresenta un oggetto DataTable di un DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/gridworksheet/datasource/) { get; set; } | Ottiene o imposta il DataSource. Generalmente è un oggetto DataSet. |
| [DisplayRightToLeft](../../aspose.cells.gridweb.data/gridworksheet/displayrighttoleft/) { get; set; } | Indica se il foglio di lavoro specificato è visualizzato da destra a sinistra invece che da sinistra a destra. Il valore predefinito è false. |
| [DisplayZeros](../../aspose.cells.gridweb.data/gridworksheet/displayzeros/) { get; set; } | True se i valori zero sono visualizzati. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/gridworksheet/enablecreatebindcolumnheader/) { get; set; } | In modalità data-binding, indica se creare le didascalie delle intestazioni di colonna di binding nel foglio. |
| [FirstVisibleColumn](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblecolumn/) { get; set; } | Rappresenta l'indice della prima colonna visibile. |
| [FirstVisibleRow](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblerow/) { get; set; } | Rappresenta l'indice della prima riga visibile. |
| [GridActiveCell](../../aspose.cells.gridweb.data/gridworksheet/gridactivecell/) { get; set; } | Ottiene o imposta la cella attiva nel foglio di lavoro. |
| [Hyperlinks](../../aspose.cells.gridweb.data/gridworksheet/hyperlinks/) { get; } | Ottiene la collezione [`GridHyperlinkCollection`](../gridhyperlinkcollection/). |
| [Index](../../aspose.cells.gridweb.data/gridworksheet/index/) { get; } | Ottiene l'indice del foglio nella collezione dei fogli di lavoro. |
| [IsGridlinesVisible](../../aspose.cells.gridweb.data/gridworksheet/isgridlinesvisible/) { get; set; } | Ottiene o imposta un valore che indica se le linee della griglia sono visibili. Il valore predefinito è true. |
| [IsSummaryRowBelow](../../aspose.cells.gridweb.data/gridworksheet/issummaryrowbelow/) { get; set; } | Indica se la riga di riepilogo sarà posizionata sotto le righe di dettaglio nella struttura. |
| [Name](../../aspose.cells.gridweb.data/gridworksheet/name/) { get; set; } | Ottiene o imposta il nome del foglio di lavoro. |
| [OutlineShown](../../aspose.cells.gridweb.data/gridworksheet/outlineshown/) { get; set; } | Indica se mostrare il contorno. |
| [Pictures](../../aspose.cells.gridweb.data/gridworksheet/pictures/) { get; } | Ottiene una collezione [`Pictures`](./pictures/). |
| [PivotTables](../../aspose.cells.gridweb.data/gridworksheet/pivottables/) { get; } | Ottiene le pivotTable nel foglio di lavoro. |
| [Selected](../../aspose.cells.gridweb.data/gridworksheet/selected/) { get; set; } | Indica se questo foglio di lavoro è selezionato quando la cartella di lavoro viene aperta. |
| [Shapes](../../aspose.cells.gridweb.data/gridworksheet/shapes/) { get; } | Ottiene una collezione [`Pictures`](./pictures/). |
| [StandardHeight](../../aspose.cells.gridweb.data/gridworksheet/standardheight/) { get; set; } | Ottiene o imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridworksheet/standardheightpixels/) { get; set; } | Ottiene o imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di pixel. |
| [TabColor](../../aspose.cells.gridweb.data/gridworksheet/tabcolor/) { get; set; } | Rappresenta il colore della scheda del foglio di lavoro. |
| [Validations](../../aspose.cells.gridweb.data/gridworksheet/validations/) { get; } | Ottiene la collezione delle impostazioni di convalida dei dati nel foglio di lavoro. |
| override [Visible](../../aspose.cells.gridweb.data/gridworksheet/visible/) { get; set; } | Indica se il nome di questo foglio è mostrato nelle schede del foglio del controllo. |
| [Workbook](../../aspose.cells.gridweb.data/gridworksheet/workbook/) { get; } | Ottiene l'oggetto [`GridWorkbook`](../gridworkbook/) della collezione di fogli di lavoro. |
| [Zoom](../../aspose.cells.gridweb.data/gridworksheet/zoom/) { get; set; } | Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/addautofilter/)(int, int, int) | Imposta l'intervallo a cui si applica l'AutoFiltro specificato. |
| [AddCustomFilter](../../aspose.cells.gridweb.data/gridworksheet/addcustomfilter/)(int, string) | Aggiunge un filtro personalizzato per la riga specificata. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn)(int) | Adatta automaticamente la larghezza della colonna. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Adatta automaticamente la larghezza della colonna. |
| [AutoFitColumns](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumns/)() |  |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow)(int) | Adatta automaticamente l'altezza della riga. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_1)(int, int, int) | Adatta automaticamente l'altezza della riga. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_2)(int, int, int, int) | Adatta automaticamente l'altezza della riga in un intervallo rettangolare. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows)() | Adatta automaticamente tutte le righe in questo foglio di lavoro. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_1)(bool) | Adatta automaticamente tutte le righe in questo foglio di lavoro. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_2)(int, int) | Adatta automaticamente l'altezza della riga in un intervallo. |
| [CalculateFormula](../../aspose.cells.gridweb.data/gridworksheet/calculateformula/)(string) | Calcola una formula. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/cancelnewbindrow/)() | Annulla ed elimina la nuova riga di binding aggiunta. |
| [ClearComments](../../aspose.cells.gridweb.data/gridworksheet/clearcomments/)() | Cancella tutti i commenti nel foglio di calcolo del designer. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/commitnewbindrow/)() | Conferma la nuova riga di binding aggiunta e la aggiunge al datasource. |
| [Copy](../../aspose.cells.gridweb.data/gridworksheet/copy/)(GridWorksheet) | Copia contenuti e formati da un altro foglio di lavoro. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/gridworksheet/createautogenratedcolumns/)() | Dopo aver impostato un datasource per il foglio di lavoro, chiama questo metodo per generare automaticamente le colonne di binding. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/createnewbindrow/)() | Crea una nuova riga di binding e la associa al datasource. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal)(int, int, int, SubtotalFunction, int[]) | Crea un subtotale nel foglio. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal_1)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Crea un subtotale nel foglio. |
| override [DataBind](../../aspose.cells.gridweb.data/gridworksheet/databind/)() | Associa il foglio al DataSource. |
| [DataSourceControlUpdate](../../aspose.cells.gridweb.data/gridworksheet/datasourcecontrolupdate/)(AccessDataSource) | Associa il foglio al DataSource. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/gridworksheet/deletebindrow/)(int) | Elimina una riga di binding. |
| [FilterString](../../aspose.cells.gridweb.data/gridworksheet/filterstring/)(int, string) | Imposta il filtro per la colonna. Nota: dobbiamo chiamare AddAutoFilter prima della chiamata a filterString. La stringa dei criteri di filtro. Nota: usiamo la virgola-&gt;\",\" come carattere di separazione, quindi il valore della cella da filtrare non deve contenere virgole. filterString(10,\"123,456\") significa che la colonna 10 deve contenere 123 o 456, filterString(10,\"123\") significa che la colonna 10 deve contenere 123. L'indice della colonna è separato da virgole, es. 123,456,789 o abc |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes_1)(string, int, int) | Blocca i riquadri nella cella specificata nel foglio di lavoro. |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes)(int, int, int, int) | Blocca i riquadri nella cella specificata nel foglio di lavoro. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/getcolumncaption/)(int) | Ottiene la didascalia della colonna. Se la didascalia non è impostata, restituisce una stringa vuota. |
| [GetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getcolumnheadertooltip/)(int) | Ottiene il testo del tooltip dell'intestazione di colonna. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/getcolumnreadonly/)(int) | Ottiene se una colonna è di sola lettura. Questo è un metodo esteso di GridWeb specificamente, non verrà mantenuto né avrà effetto nel file Excel reale. |
| [GetFreezedPanes](../../aspose.cells.gridweb.data/gridworksheet/getfreezedpanes/)(out int, out int, out int, out int) | Ottiene i riquadri congelati. |
| [GetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/getisreadonly/)(int, int) | Ottiene se la cella è di sola lettura. Questo è un attributo esteso di GridWeb, non verrà mantenuto nel file Excel reale. |
| [GetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/getrowcaption/)(int) | Ottiene la didascalia della riga. Se la didascalia non è impostata, restituisce una stringa vuota. |
| [GetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getrowheadertooltip/)(int) | Ottiene il testo del tooltip dell'intestazione di riga. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/getrowreadonly/)(int) | Ottiene se una riga è di sola lettura. questo è un metodo esteso di GridWeb specificamente, non verrà mantenuto né avrà effetto nel file Excel reale |
| [GroupRows](../../aspose.cells.gridweb.data/gridworksheet/grouprows/)(int, int, bool) | Raggruppa le righe. |
| [IsProtected](../../aspose.cells.gridweb.data/gridworksheet/isprotected/)() | Indica se il foglio di lavoro è protetto. |
| [MoveTo](../../aspose.cells.gridweb.data/gridworksheet/moveto/)(int) | Sposta il foglio in un'altra posizione nel foglio di calcolo. |
| [RefreshFilter](../../aspose.cells.gridweb.data/gridworksheet/refreshfilter/)() | Aggiorna i filtri automatici per nascondere o mostrare le righe. |
| [RemoveAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/removeautofilter/)() | Rimuove il filtro automatico del foglio di lavoro. |
| [RemoveSubtotal](../../aspose.cells.gridweb.data/gridworksheet/removesubtotal/)() | Rimuove il subtotale creato dal metodo CreateSubtotal nel foglio. |
| [ResetFilter](../../aspose.cells.gridweb.data/gridworksheet/resetfilter/)(int) | L'offset intero del campo su cui si desidera applicare, basato sulla prima colonna di filtro (da sinistra nella lista; il campo più a sinistra è il campo 0). |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/gridworksheet/setallcellseditable/)() | Rende tutte le celle modificabili. questo è un attributo esteso |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setallcellsreadonly/)() | Rende tutte le celle di sola lettura. questo è un attributo esteso, nota che questo attributo non può essere mantenuto nella cella reale; se desideri mantenere la protezione, usa setProtect |
| [SetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/setcolumncaption/)(int, string) | Imposta la didascalia per la colonna. si prega di notare che questo è un attributo di estensione e non può essere mantenuto nel file Excel |
| [SetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setcolumnheadertooltip/)(int, string) | Imposta il testo del tooltip dell'intestazione di colonna. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/setcolumnreadonly/)(int, bool) | Imposta una colonna come di sola lettura così l'utente non può eliminarla dal lato client. questo è un metodo esteso di GridWeb specificamente, non verrà mantenuto né avrà effetto nel file Excel reale |
| [SetEditableRange](../../aspose.cells.gridweb.data/gridworksheet/seteditablerange/)(int, int, int, int) | Rende modificabile un intervallo di celle. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Rendi tutte le celle di sola lettura chiamando il metodo SetAllCellsReadonly. poi chiama questo metodo per specificare l'intervallo di celle da rendere modificabile |
| [SetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setisreadonly/)(int, int, bool) | Imposta se la cella è di sola lettura. questo è un attributo esteso di GridWeb, non verrà mantenuto nel file Excel reale |
| [SetProtect](../../aspose.cells.gridweb.data/gridworksheet/setprotect/)() | Protegge il worksheet. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/gridworksheet/setreadonlyrange/)(int, int, int, int) | Rende un intervallo di celle di sola lettura. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Prima rendi tutte le celle modificabili chiamando il metodo SetAllCellsEditable. poi chiama questo metodo per specificare l'intervallo di celle da rendere di sola lettura |
| [SetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/setrowcaption/)(int, string) | Imposta la didascalia per la riga. |
| [SetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setrowheadertooltip/)(int, string) | Imposta il testo del tooltip dell'intestazione di riga. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/setrowreadonly/)(int, bool) | Imposta una riga come di sola lettura così l'utente non può eliminarla dal lato client. questo è un metodo esteso di GridWeb specificamente, non verrà mantenuto né avrà effetto nel file Excel reale |
| [UnFreezePanes](../../aspose.cells.gridweb.data/gridworksheet/unfreezepanes/)() | Sblocca i riquadri nel worksheet. |
| [UnGroupRows](../../aspose.cells.gridweb.data/gridworksheet/ungrouprows/)(int, int) | Separa le righe dal raggruppamento. |
| [UnProtect](../../aspose.cells.gridweb.data/gridworksheet/unprotect/)() | Rimuove la protezione del foglio di lavoro. |

## Eventi

| Nome | Descrizione |
| --- | --- |
| event [InitializeNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/initializenewbindrow/) | Si verifica quando il foglio di lavoro ha creato una nuova riga di binding e necessita di inizializzarla. |

### Vedi anche

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


