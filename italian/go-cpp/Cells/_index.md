---
title: "Classe Cells"
linktitle: "Cells"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe Cells. Incapsula l'oggetto che rappresenta le celle in Go."
type: docs
weight: 200
url: /it/go-cpp/cells/
---

## Cells class

Incapsula una collezione di oggetti rilevanti per la cella, come <see cref=\"Cell\"/>, <see cref=\"Row\"/>, ...ecc.

```go

type Cells struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetOdsCellFields](./getodscellfields/) | Ottiene l'elenco dei campi di ods. |
| [Dispose](./dispose/) | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino delle risorse non gestite. |
| [GetCount](./getcount/) | Ottiene il conteggio totale degli oggetti Cell istanziati. |
| [GetCountLarge](./getcountlarge/) | Ottiene il conteggio totale degli oggetti Cell istanziati. |
| [GetEnumerator](./getenumerator/) | Ottiene l'enumeratore delle celle. |
| [GetRows](./getrows/) | Ottiene la collezione di oggetti Row che rappresenta le righe individuali in questo foglio di lavoro. |
| [GetMergedAreas](./getmergedareas/) | Ottiene tutte le celle unite. |
| [CheckCell](./checkcell/) | Ottiene l'elemento Cell o null all'indice di riga e colonna della cella specificati. |
| [CheckRow](./checkrow/) | Ottiene l'elemento Row o null all'indice di riga della cella specificato. |
| [CheckColumn](./checkcolumn/) | Ottiene l'elemento Column o null all'indice di colonna specificato. |
| [IsRowHidden](./isrowhidden/) | Verifica se una riga all'indice specificato è nascosta. |
| [IsColumnHidden](./iscolumnhidden/) | Verifica se una colonna all'indice specificato è nascosta. |
| [AddRange](./addrange/) | Aggiunge un riferimento a un oggetto intervallo alle celle |
| [CreateRange_String_String](./createrange_string_string/) | Crea un oggetto Range da un intervallo di celle. |
| [CreateRange_Int_Int_Int_Int](./createrange_int_int_int_int/) | Crea un oggetto Range da un intervallo di celle. |
| [CreateRange_String](./createrange_string/) | Crea un oggetto Range da un indirizzo dell'intervallo. |
| [CreateRange_Int_Int_Bool](./createrange_int_int_bool/) | Crea un oggetto Range da righe di celle o colonne di celle. |
| [Get_Int_Int](./get_int_int/) | Ottiene l'elemento Cell all'indice di riga e colonna della cella specificati. |
| [Get_String](./get_string/) | Ottiene l'elemento Cell al nome della cella specificato. |
| [GetMultiThreadReading](./getmultithreadreading/) | Ottiene o imposta se il modello dati delle celle deve supportare la lettura multi-thread. Il valore predefinito di questa proprietà è false. |
| [SetMultiThreadReading](./setmultithreadreading/) | Ottiene o imposta se il modello dati delle celle deve supportare la lettura multi-thread. Il valore predefinito di questa proprietà è false. |
| [GetMemorySetting](./getmemorysetting/) | Ottiene o imposta l'opzione di utilizzo della memoria per queste celle. |
| [SetMemorySetting](./setmemorysetting/) | Ottiene o imposta l'opzione di utilizzo della memoria per queste celle. |
| [Clear](./clear/) | Cancella tutti i dati del foglio di lavoro. |
| [GetStyle](./getstyle/) | Ottiene e imposta lo stile predefinito del foglio di lavoro. |
| [SetStyle](./setstyle/) | Ottiene e imposta lo stile predefinito del foglio di lavoro. |
|[IsDefaultColumnHidden](./isdefaultcolumnhidden/) |  | 
|[SetIsDefaultColumnHidden](./setisdefaultcolumnhidden/) |  | 
| [GetStandardWidthInch](./getstandardwidthinch/) | Ottiene o imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di pollici. |
| [SetStandardWidthInch](./setstandardwidthinch/) | Ottiene o imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di pollici. |
| [GetStandardWidthPixels](./getstandardwidthpixels/) | Ottiene o imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di pixel. |
| [SetStandardWidthPixels](./setstandardwidthpixels/) | Ottiene o imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di pixel. |
| [GetStandardWidth](./getstandardwidth/) | Ottiene o imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di caratteri. |
| [SetStandardWidth](./setstandardwidth/) | Ottiene o imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di caratteri. |
| [GetStandardHeight](./getstandardheight/) | Ottiene o imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti. |
| [SetStandardHeight](./setstandardheight/) | Ottiene o imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti. |
| [GetStandardHeightPixels](./getstandardheightpixels/) | Ottiene o imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di pixel. |
| [SetStandardHeightPixels](./setstandardheightpixels/) | Ottiene o imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di pixel. |
| [GetStandardHeightInch](./getstandardheightinch/) | Ottiene o imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di pollici. |
| [SetStandardHeightInch](./setstandardheightinch/) | Ottiene o imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di pollici. |
| [ImportFormulaArray](./importformulaarray/) | Importa un array di formule in un foglio di lavoro. |
| [TextToColumns](./texttocolumns/) | Divide il contenuto nella colonna specificata in più colonne. |
| [ImportCSV_String_String_Bool_Int_Int](./importcsv_string_string_bool_int_int/) | Importa un file CSV nelle celle. |
| [ImportCSV_Stream_String_Bool_Int_Int](./importcsv_stream_string_bool_int_int/) | Importa un file CSV nelle celle. |
| [ImportCSV_String_TxtLoadOptions_Int_Int](./importcsv_string_txtloadoptions_int_int/) | Importa un file CSV nelle celle. |
| [ImportCSV_Stream_TxtLoadOptions_Int_Int](./importcsv_stream_txtloadoptions_int_int/) | Importa un file CSV nelle celle. |
| [GetPreserveString](./getpreservestring/) | Ottiene o imposta un valore che indica se tutti i valori del foglio di lavoro sono conservati come stringhe. Il valore predefinito è false. |
| [SetPreserveString](./setpreservestring/) | Ottiene o imposta un valore che indica se tutti i valori del foglio di lavoro sono conservati come stringhe. Il valore predefinito è false. |
| [Merge_Int_Int_Int_Int](./merge_int_int_int_int/) | Unisce un intervallo specificato di celle in una singola cella. |
| [Merge_Int_Int_Int_Int_Bool](./merge_int_int_int_int_bool/) | Unisce un intervallo specificato di celle in una singola cella. |
| [Merge_Int_Int_Int_Int_Bool_Bool](./merge_int_int_int_int_bool_bool/) | Unisce un intervallo specificato di celle in una singola cella. |
| [UnMerge](./unmerge/) | Separa un intervallo specificato di celle unite. |
| [ClearMergedCells](./clearmergedcells/) | Cancella tutti gli intervalli uniti. |
| [HideRow](./hiderow/) | Nasconde una riga. |
| [UnhideRow](./unhiderow/) | Rivela una riga. |
| [HideRows](./hiderows/) | Nasconde più righe. |
| [UnhideRows](./unhiderows/) | Rivela le righe nascoste. |
| [SetRowHeightPixel](./setrowheightpixel/) | Imposta l'altezza della riga in unità di pixel. |
| [SetRowHeightInch](./setrowheightinch/) | Imposta l'altezza della riga in unità di pollici. |
| [SetRowHeight](./setrowheight/) | Imposta l'altezza della riga specificata. |
| [GetRowHeight_Int_Bool_CellsUnitType](./getrowheight_int_bool_cellsunittype/) | Ottiene l'altezza della riga. |
| [GetColumnWidth_Int_Bool_CellsUnitType](./getcolumnwidth_int_bool_cellsunittype/) | Ottiene la larghezza della colonna. |
| [HideColumn](./hidecolumn/) | Nasconde una colonna. |
| [UnhideColumn](./unhidecolumn/) | Rivela una colonna |
| [HideColumns](./hidecolumns/) | Nascondi più colonne. |
| [UnhideColumns](./unhidecolumns/) | Rivela più colonne. |
| [GetRowHeight_Int](./getrowheight_int/) | Ottiene l'altezza di una riga specificata, in unità di punti. |
| [GetViewRowHeight](./getviewrowheight/) | Ottiene l'altezza di una riga specificata. |
| [GetRowHeightInch](./getrowheightinch/) | Ottiene l'altezza di una riga specificata in unità di pollici. |
| [GetViewRowHeightInch](./getviewrowheightinch/) | Ottiene l'altezza di una riga specificata in unità di pollici. |
| [GetRowHeightPixel](./getrowheightpixel/) | Ottiene l'altezza di una riga specificata in unità di pixel. |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | Imposta la larghezza della colonna in unità di pixel nella visualizzazione normale. |
| [SetColumnWidthInch](./setcolumnwidthinch/) | Imposta la larghezza della colonna in unità di pollici nella visualizzazione normale. |
| [SetColumnWidth](./setcolumnwidth/) | Imposta la larghezza della colonna specificata nella visualizzazione normale. |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | Ottiene la larghezza della colonna specificata nella visualizzazione normale, in unità di pixel. |
| [GetColumnWidth_Int](./getcolumnwidth_int/) | Ottiene la larghezza (in unità di caratteri) della colonna specificata nella visualizzazione normale |
| [GetViewColumnWidthPixel](./getviewcolumnwidthpixel/) | Ottieni la larghezza in diversi tipi di visualizzazione. |
| [SetViewColumnWidthPixel](./setviewcolumnwidthpixel/) | Imposta la larghezza della colonna in diverse visualizzazioni. |
| [GetMinRow](./getminrow/) | Indice minimo di riga della cella che contiene dati o stile. |
| [GetMaxRow](./getmaxrow/) | Indice massimo di riga della cella che contiene dati o stile. |
| [GetMinColumn](./getmincolumn/) | Indice minimo di colonna delle celle che sono state istanziate nella raccolta (non include la colonna in cui lo stile è definito per l'intera colonna ma nessuna cella è stata istanziata in essa). |
| [GetMaxColumn](./getmaxcolumn/) | Indice massimo della colonna delle celle che sono state istanziate nella collezione (non include la colonna in cui lo stile è definito per l'intera colonna ma nessuna cella è stata istanziata in essa). |
| [GetMinDataRow](./getmindatarow/) | Indice minimo della riga della cella che contiene dati. |
| [GetMaxDataRow](./getmaxdatarow/) | Indice massimo della riga della cella che contiene dati. |
| [GetMinDataColumn](./getmindatacolumn/) | Indice minimo della colonna della cella che contiene dati. |
| [GetMaxDataColumn](./getmaxdatacolumn/) | Indice massimo della colonna della cella che contiene dati. |
| [GetLastDataRow](./getlastdatarow/) | Restituisce l'indice dell'ultima riga della cella che contiene dati nella colonna specificata. |
| [GetFirstDataRow](./getfirstdatarow/) | Restituisce l'indice della prima riga della cella che contiene dati nella colonna specificata. |
| [IsDefaultRowHeightMatched](./isdefaultrowheightmatched/) | Indica che l'altezza della riga e l'altezza predefinita del carattere corrispondono |
| [SetIsDefaultRowHeightMatched](./setisdefaultrowheightmatched/) | Indica che l'altezza della riga e l'altezza predefinita del carattere corrispondono |
| [IsDefaultRowHidden](./isdefaultrowhidden/) | Indica se la riga è nascosta per impostazione predefinita. |
| [SetIsDefaultRowHidden](./setisdefaultrowhidden/) | Indica se la riga è nascosta per impostazione predefinita. |
| [GetColumns](./getcolumns/) | Restituisce la collezione di oggetti Column che rappresentano le singole colonne in questo foglio di lavoro. |
| [ApplyColumnStyle](./applycolumnstyle/) | Applica formati a un'intera colonna. |
| [ApplyRowStyle](./applyrowstyle/) | Applica formati a un'intera riga. |
| [ApplyStyle](./applystyle/) | Applica formati a un intero foglio di lavoro. |
| [CopyColumns_Cells_Int_Int_Int_PasteOptions](./copycolumns_cells_int_int_int_pasteoptions/) | Copia dati e formati di un'intera colonna. |
| [CopyColumn](./copycolumn/) | Copia dati e formati di un'intera colonna. |
| [CopyColumns_Cells_Int_Int_Int](./copycolumns_cells_int_int_int/) | Copia dati e formati di intere colonne. |
| [CopyColumns_Cells_Int_Int_Int_Int](./copycolumns_cells_int_int_int_int/) | Copia dati e formati delle intere colonne. |
| [CopyRow](./copyrow/) | Copia dati e formati di un'intera riga. |
| [CopyRows_Cells_Int_Int_Int](./copyrows_cells_int_int_int/) | Copia dati e formati di alcune intere righe. |
| [CopyRows_Cells_Int_Int_Int_CopyOptions](./copyrows_cells_int_int_int_copyoptions/) | Copia dati e formati di alcune intere righe. |
| [CopyRows_Cells_Int_Int_Int_CopyOptions_PasteOptions](./copyrows_cells_int_int_int_copyoptions_pasteoptions/) | Copia dati e formati di alcune intere righe. |
| [GetGroupedRowOutlineLevel](./getgroupedrowoutlinelevel/) | Restituisce il livello di outline (basato su zero) della riga. |
| [GetGroupedColumnOutlineLevel](./getgroupedcolumnoutlinelevel/) | Restituisce il livello di outline (basato su zero) della colonna. |
| [GetMaxGroupedColumnOutlineLevel](./getmaxgroupedcolumnoutlinelevel/) | Restituisce il livello massimo di outline delle colonne raggruppate (basato su zero). |
| [GetMaxGroupedRowOutlineLevel](./getmaxgroupedrowoutlinelevel/) | Restituisce il livello massimo di outline delle righe raggruppate (basato su zero). |
| [ShowGroupDetail](./showgroupdetail/) | Espande le righe/colonne raggruppate. |
| [HideGroupDetail](./hidegroupdetail/) | Comprimi le righe/colonne raggruppate. |
| [UngroupColumns](./ungroupcolumns/) | Separa le colonne. |
| [GroupColumns_Int_Int](./groupcolumns_int_int/) | Raggruppa colonne. |
| [GroupColumns_Int_Int_Bool](./groupcolumns_int_int_bool/) | Raggruppa colonne. |
| [UngroupRows_Int_Int_Bool](./ungrouprows_int_int_bool/) | Separa righe. |
| [UngroupRows_Int_Int](./ungrouprows_int_int/) | Separa righe. |
| [GroupRows_Int_Int_Bool](./grouprows_int_int_bool/) | Raggruppa righe. |
| [GroupRows_Int_Int](./grouprows_int_int/) | Raggruppa righe. |
| [DeleteColumn_Int_Bool](./deletecolumn_int_bool/) | Elimina una colonna. |
| [DeleteColumn_Int](./deletecolumn_int/) | Elimina una colonna. |
| [DeleteColumns_Int_Int_Bool](./deletecolumns_int_int_bool/) | Elimina diverse colonne. |
| [DeleteColumns_Int_Int_DeleteOptions](./deletecolumns_int_int_deleteoptions/) | Elimina diverse colonne. |
| [IsDeletingRangeEnabled](./isdeletingrangeenabled/) | Verifica se l'intervallo può essere eliminato. |
| [DeleteRow_Int](./deleterow_int/) | Elimina una riga. |
| [DeleteRow_Int_Bool](./deleterow_int_bool/) | Elimina una riga. |
| [DeleteRows_Int_Int](./deleterows_int_int/) | Elimina più righe. |
| [DeleteRows_Int_Int_Bool](./deleterows_int_int_bool/) | Elimina più righe nel foglio di lavoro. |
| [DeleteRows_Int_Int_DeleteOptions](./deleterows_int_int_deleteoptions/) | Elimina più righe nel foglio di lavoro. |
| [DeleteBlankColumns](./deleteblankcolumns/) | Elimina tutte le colonne vuote che non contengono dati. |
| [DeleteBlankColumns_DeleteOptions](./deleteblankcolumns_deleteoptions/) | Elimina tutte le colonne vuote che non contengono dati. |
| [IsBlankColumn](./isblankcolumn/) | Verifica se la colonna fornita è vuota (non contiene dati). |
| [DeleteBlankRows](./deleteblankrows/) | Elimina tutte le righe vuote che non contengono dati o altri oggetti. |
| [DeleteBlankRows_DeleteOptions](./deleteblankrows_deleteoptions/) | Elimina tutte le righe vuote che non contengono dati o alcuni oggetti speciali come commenti visibili, tabelle pivot. |
| [InsertColumns_Int_Int](./insertcolumns_int_int/) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertColumns_Int_Int_Bool](./insertcolumns_int_int_bool/) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertColumns_Int_Int_InsertOptions](./insertcolumns_int_int_insertoptions/) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertColumn_Int_Bool](./insertcolumn_int_bool/) | Inserisce una nuova colonna nel foglio di lavoro. |
| [InsertColumn_Int](./insertcolumn_int/) | Inserisce una nuova colonna nel foglio di lavoro. |
| [InsertRows_Int_Int_Bool](./insertrows_int_int_bool/) | Inserisce più righe nel foglio di lavoro. |
| [InsertRows_Int_Int_InsertOptions](./insertrows_int_int_insertoptions/) | Inserisce più righe nel foglio di lavoro. |
| [InsertRows_Int_Int](./insertrows_int_int/) | Inserisce più righe nel foglio di lavoro. |
| [InsertRow](./insertrow/) | Inserisce una nuova riga nel foglio di lavoro. |
| [GetRanges](./getranges/) | Ottiene la collezione di oggetti Range creati a runtime. |
| [ClearRange_CellArea](./clearrange_cellarea/) | Cancella il contenuto e la formattazione di un intervallo. |
| [ClearRange_Int_Int_Int_Int](./clearrange_int_int_int_int/) | Cancella il contenuto e la formattazione di un intervallo. |
| [ClearContents_CellArea](./clearcontents_cellarea/) | Cancella il contenuto di un intervallo. |
| [ClearContents_Int_Int_Int_Int](./clearcontents_int_int_int_int/) | Cancella il contenuto di un intervallo. |
| [ClearFormats_CellArea](./clearformats_cellarea/) | Cancella la formattazione di un intervallo. |
| [ClearFormats_Int_Int_Int_Int](./clearformats_int_int_int_int/) | Cancella la formattazione di un intervallo. |
| [GetLastCell](./getlastcell/) | Ottiene l'ultima cella in questo foglio di lavoro. |
| [LinkToXmlMap](./linktoxmlmap/) | Collegamento a una mappa XML. |
| [GetMaxDisplayRange](./getmaxdisplayrange/) | Ottiene l'intervallo massimo che include dati, celle unite e forme. |
| [GetFirstCell](./getfirstcell/) | Ottiene la prima cella in questo foglio di lavoro. |
| [Find_Object_Cell](./find_object_cell/) | Trova la cella contenente l'oggetto di input. |
| [Find_Object_Cell_FindOptions](./find_object_cell_findoptions/) | Trova la cella contenente l'oggetto di input. |
| [EndCellInRow_Int](./endcellinrow_int/) | Ottiene l'ultima cella in questa riga. |
| [EndCellInColumn_Int](./endcellincolumn_int/) | Ottiene l'ultima cella in questa colonna. |
| [EndCellInColumn_Int_Int_Int_Int](./endcellincolumn_int_int_int_int/) | Ottiene l'ultima cella con indice di colonna massimo in questo intervallo. |
| [EndCellInRow_Int_Int_Int_Int](./endcellinrow_int_int_int_int/) | Ottiene l'ultima cella con indice di riga massimo in questo intervallo. |
| [MoveRange](./moverange/) | Sposta l'intervallo. |
| [InsertCutCells](./insertcutcells/) | Inserisci l'intervallo tagliato. |
| [InsertRange_CellArea_Int_ShiftType_Bool](./insertrange_cellarea_int_shifttype_bool/) | Inserisce un intervallo di celle e sposta le celle secondo l'opzione di spostamento. |
| [InsertRange_CellArea_ShiftType](./insertrange_cellarea_shifttype/) | Inserisce un intervallo di celle e sposta le celle secondo l'opzione di spostamento. |
| [InsertRange_CellArea_Int_ShiftType](./insertrange_cellarea_int_shifttype/) | Inserisce un intervallo di celle e sposta le celle secondo l'opzione di spostamento. |
| [DeleteRange](./deleterange/) | Elimina un intervallo di celle e sposta le celle secondo l'opzione di spostamento. |
| [ExportArray](./exportarray/) | Esporta i dati nella raccolta Cells in un oggetto array bidimensionale. |
| [RetrieveSubtotalSetting](./retrievesubtotalsetting/) | Recupera le impostazioni dei subtotali dell'intervallo. |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array](./subtotal_cellarea_int_consolidationfunction_int32array/) | Crea subtotali per l'intervallo. |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array_Bool_Bool_Bool](./subtotal_cellarea_int_consolidationfunction_int32array_bool_bool_bool/) | Crea subtotali per l'intervallo. |
| [RemoveFormulas](./removeformulas/) | Rimuove tutte le formule e le sostituisce con il valore della formula. |
| [RemoveDuplicates](./removeduplicates/) | Rimuove le righe duplicate nel foglio. |
| [RemoveDuplicates_Int_Int_Int_Int](./removeduplicates_int_int_int_int/) | Rimuove i valori duplicati nell'intervallo. |
| [RemoveDuplicates_Int_Int_Int_Int_Bool_int32Array](./removeduplicates_int_int_int_int_bool_int32array/) | Rimuove i dati duplicati dell'intervallo. |
| [ConvertStringToNumericValue](./convertstringtonumericvalue/) | Converte tutti i dati stringa nel foglio di lavoro in valori numerici, se possibile. |
| [GetDependents](./getdependents/) | Ottieni tutte le celle che fanno riferimento alla cella specifica. |
| [GetDependentsInCalculation](./getdependentsincalculation/) | Ottiene tutte le celle il cui risultato calcolato dipende dalla cella specifica. |
| [GetCellsWithPlaceInCellPicture](./getcellswithplaceincellpicture/) | Ottiene tutte le celle che contengono un'immagine incorporata. |
| [GetCellStyle](./getcellstyle/) | Ottieni lo stile della cella fornita. |
| [GetCellDisplayStyle_Int_Int](./getcelldisplaystyle_int_int/) | Ottieni lo stile di visualizzazione della cella fornita. |
| [GetCellDisplayStyle_Int_Int_BorderType](./getcelldisplaystyle_int_int_bordertype/) | Ottieni lo stile di visualizzazione della cella fornita. |
