---
title: "Classe Range"
linktitle: "Range"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe Range. Incapsula l'oggetto che rappresenta range in Go."
type: docs
weight: 200
url: /it/go-cpp/range/
---

## Range class

Incapsula l'oggetto che rappresenta un intervallo di celle all'interno di un foglio di calcolo.

```go

type Range struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewRange_CellArea_Cells](./newrange_cellarea_cells/) | Costruttore della classe. |
| [NewRange_Int_Int_Int_Int_Cells](./newrange_int_int_int_int_cells/) | Costruttore della classe. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [AutoFill_Range](./autofill_range/) | Riempie automaticamente l'intervallo di destinazione. |
| [AutoFill_Range_AutoFillType](./autofill_range_autofilltype/) | Riempie automaticamente l'intervallo di destinazione. |
| [GetCurrentRegion](./getcurrentregion/) | Restituisce un oggetto Range che rappresenta la regione corrente. La regione corrente è un intervallo delimitato da qualsiasi combinazione di righe vuote e colonne vuote. |
| [GetHyperlinks](./gethyperlinks/) | Ottiene tutti i collegamenti ipertestuali nell'intervallo. |
| [AddHyperlink](./addhyperlink/) | Aggiunge un collegamento ipertestuale a una cella specificata o a un intervallo di celle. |
| [GetEnumerator](./getenumerator/) | Ottiene l'enumeratore per le celle in questo Range. |
| [IsIntersect](./isintersect/) | Indica se l'intervallo si interseca. |
| [Intersect](./intersect/) | Restituisce un oggetto Range che rappresenta l'intersezione rettangolare di due intervalli. |
| [UnionRanges](./unionranges/) | Restituisce il risultato dell'unione di due intervalli. |
| [GetRowCount](./getrowcount/) | Ottiene il conteggio delle righe nell'intervallo. |
| [GetColumnCount](./getcolumncount/) | Ottiene il conteggio delle colonne nell'intervallo. |
| [GetName](./getname/) | Ottiene o imposta il nome dell'intervallo. |
| [SetName](./setname/) | Ottiene o imposta il nome dell'intervallo. |
| [GetRefersTo](./getrefersto/) | Ottiene a cosa si riferisce l'intervallo. |
| [GetAddress](./getaddress/) | Ottiene l'indirizzo dell'intervallo. |
| [IsBlank](./isblank/) | Indica se l'intervallo contiene valori. |
| [GetLeft](./getleft/) | Restituisce la distanza, in punti, dal bordo sinistro della colonna A al bordo sinistro dell'intervallo. |
| [GetTop](./gettop/) | Restituisce la distanza, in punti, dal bordo superiore della riga 1 al bordo superiore dell'intervallo. |
| [GetWidth](./getwidth/) | Restituisce la larghezza di un intervallo in punti. |
| [GetHeight](./getheight/) | Restituisce la larghezza di un intervallo in punti. |
| [GetFirstRow](./getfirstrow/) | Restituisce l'indice della prima riga dell'intervallo. |
| [GetFirstColumn](./getfirstcolumn/) | Restituisce l'indice della prima colonna dell'intervallo. |
| [Merge](./merge/) | Combina un intervallo di celle in una singola cella. |
| [UnMerge](./unmerge/) | Separa le celle unite di questo intervallo. |
| [PutValue](./putvalue/) | Inserisce un valore nell'intervallo; se opportuno il valore verrà convertito in un altro tipo di dato e il formato numerico della cella verrà ripristinato. |
| [GetValue](./getvalue/) | Ottiene e imposta il valore dell'intervallo. |
| [SetValue](./setvalue/) | Ottiene e imposta il valore dell'intervallo. |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | Applica lo stile della cella. |
| [ApplyStyle](./applystyle/) | Applica formati a un intero intervallo. |
| [SetStyle_Style](./setstyle_style/) | Imposta lo stile dell'intervallo. |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | Imposta i bordi di contorno attorno a un intervallo di celle con lo stesso stile e colore del bordo. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Imposta i bordi di contorno attorno a un intervallo di celle con lo stesso stile e colore del bordo. |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | Imposta i bordi di contorno attorno a un intervallo di celle. |
| [SetOutlineBorder_BorderType_CellBorderType_CellsColor](./setoutlineborder_bordertype_cellbordertype_cellscolor/) | Imposta il bordo di contorno attorno a un intervallo di celle. |
| [SetOutlineBorder_BorderType_CellBorderType_Color](./setoutlineborder_bordertype_cellbordertype_color/) | Imposta il bordo di contorno attorno a un intervallo di celle. |
| [SetInsideBorders](./setinsideborders/) | Imposta i bordi interni dell'intervallo. |
| [GetColumnWidth](./getcolumnwidth/) | Imposta o ottiene la larghezza della colonna di questo intervallo |
| [SetColumnWidth](./setcolumnwidth/) | Imposta o ottiene la larghezza della colonna di questo intervallo |
| [GetRowHeight](./getrowheight/) | Imposta o ottiene l'altezza delle righe in questo intervallo |
| [SetRowHeight](./setrowheight/) | Imposta o ottiene l'altezza delle righe in questo intervallo |
| [MoveTo](./moveto/) | Sposta l'intervallo corrente nell'intervallo di destinazione. |
| [CopyData](./copydata/) | Copia i dati delle celle (incluse le formule) da un intervallo di origine. |
| [CopyValue](./copyvalue/) | Copia il valore della cella da un intervallo di origine. |
| [CopyStyle](./copystyle/) | Copia le impostazioni di stile da un intervallo di origine. |
| [Copy_Range_PasteOptions](./copy_range_pasteoptions/) | Copia l'intervallo con le opzioni Incolla speciale. |
| [Transpose](./transpose/) | Trasponi (ruota) i dati da righe a colonne o viceversa. |
| [Copy_Range](./copy_range/) | Copia i dati (incluse le formule), la formattazione, gli oggetti di disegno ecc. da un intervallo di origine. |
| [Get](./get/) | Ottiene l'oggetto Cell in questo intervallo. |
| [GetCellOrNull](./getcellornull/) | Ottiene l'oggetto Cell o null in questo intervallo. |
| [GetOffset](./getoffset/) | Ottiene l'intervallo Range mediante offset. |
| [GetEntireColumn](./getentirecolumn/) | Ottiene un oggetto Range che rappresenta l'intera colonna (o le colonne) che contiene l'intervallo specificato. |
| [GetEntireRow](./getentirerow/) | Ottiene un oggetto Range che rappresenta l'intera riga (o le righe) che contiene l'intervallo specificato. |
| [GetWorksheet](./getworksheet/) | Ottiene l'oggetto Worksheetobject che contiene questo intervallo. |
| [ToString](./tostring/) | Restituisce una stringa che rappresenta l'oggetto Range corrente. |
| [ToImage](./toimage/) | Converte l'intervallo in immagine. |
| [ToJson](./tojson/) | Converte l'intervallo in valore JSON. |
| [ToHtml](./tohtml/) | Converte l'intervallo in HTML. |
| [Clear](./clear/) | Cancella questo intervallo. |
| [ClearContents](./clearcontents/) | Cancella il contenuto di questo intervallo. |
| [ClearFormats](./clearformats/) | Cancella i formati di questo intervallo. |
| [ClearComments](./clearcomments/) | Cancella i commenti di questo intervallo. |
| [ClearHyperlinks](./clearhyperlinks/) | Rimuove solo i collegamenti ipertestuali. |
