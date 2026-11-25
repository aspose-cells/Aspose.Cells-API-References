---
title: "Classe WorksheetDesign"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.WorksheetDesign. Ereditata da WebWorksheet. Utilizzata solo a tempo di progettazione."
type: docs
url: /it/net/aspose.cells.gridweb/worksheetdesign/
---
## WorksheetDesign class

Ereditato da WebWorksheet. Utilizzato solo a tempo di progettazione.

```csharp
public class WorksheetDesign : WebWorksheet
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WorksheetDesign](worksheetdesign/#constructor)() | Costruttore predefinito. |
| [WorksheetDesign](worksheetdesign/#constructor_1)(MainWeb, GridWorksheet) | il costruttore con MainWeb e GridWorksheet |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | Collezione di colonne Bind. (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | L'oggetto sorgente dati effettivamente collegato a runtime. È un oggetto DataView quando la proprietà DataSource è un oggetto DataSet, DataTable o DataView. (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | In modalità data-binding, BindStartRow e BindStartColumn indicano la posizione della griglia da collegare alla sorgente dati. (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | In modalità data-binding, BindStartRow e BindStartColumn indicano la posizione della griglia da collegare alla sorgente dati. (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } | (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | Restituisce il [`WebCells`](../../aspose.cells.gridweb.data/webcells/). (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } | (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | Restituisce il numero di righe di collegamento in modalità data-binding. (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | Restituisce o imposta il DataMember dalla DataSource multivalore. Generalmente rappresenta un oggetto DataTable di un DataSet. (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | Restituisce o imposta la DataSource. Generalmente è un oggetto DataSet. (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | In modalità data-binding, indica se creare le didascalie delle intestazioni di colonna collegate nel foglio. (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | Restituisce la collezione HyperlinkCollection. (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | Restituisce l'indice di se stesso all'interno dei fogli di lavoro. (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | Restituisce o imposta se il foglio di lavoro è protetto. Quando un foglio di lavoro è protetto, tutte le celle non possono essere modificate eccetto la cella la cui proprietà IsLocked è falsa. (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | Restituisce o imposta il nome del foglio. (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } | (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | Restituisce la collezione delle impostazioni di convalida dati nel foglio di lavoro. (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | Indica se il nome di questo foglio è mostrato nelle schede dei fogli del controllo. (Ereditata da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/)(int) | Adatta automaticamente la larghezza della colonna.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/)(int, int, int) | Adatta automaticamente la larghezza della colonna. Questo metodo adatta automaticamente una colonna in base al contenuto in un intervallo di celle all'interno della colonna dalla riga iniziale alla riga finale. AutoFitColumn è una funzione imprecisa.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | Annulla ed elimina la nuova riga di binding aggiunta.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | Conferma la nuova riga di binding aggiunta e la aggiunge alla fonte dati.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | Copia da un altro oggetto foglio di lavoro.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | Dopo aver impostato una fonte dati per il foglio di lavoro, chiama questo metodo per generare automaticamente le colonne di binding.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | Crea una nuova riga di binding e la associa alla fonte dati.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Crea un subtotale nel foglio.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | Associa il foglio alla fonte dati.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | Elimina una riga di binding.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | Blocca i riquadri nella cella specificata del foglio di lavoro.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/)(int, int) | Raggruppa le righe.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/)(int, int, bool) | Raggruppa le righe.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | Rende tutte le celle modificabili. questo è un attributo esteso(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | Rende tutte le celle di sola lettura. questo è un attributo esteso, nota che questo attributo non può essere mantenuto nella cella reale, se vuoi mantenere la protezione usa setProtect(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | Rende modificabile un intervallo di celle. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Rendi tutte le celle di sola lettura chiamando il metodo SetAllCellsReadonly. poi chiama questo metodo per specificare l'intervallo di celle da rendere modificabile(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | Rende di sola lettura un intervallo di celle. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Prima rendi tutte le celle modificabili chiamando il metodo SetAllCellsEditable. poi chiama questo metodo per specificare l'intervallo di celle da rendere di sola lettura(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | Sblocca i riquadri nel foglio di lavoro.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | Separa le righe raggruppate.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | Aggiorna il valore della proprietà del record della fonte dati di binding in base al valore della cella.(Ereditato da [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |

### Vedi anche

* class [WebWorksheet](../../aspose.cells.gridweb.data/webworksheet/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


