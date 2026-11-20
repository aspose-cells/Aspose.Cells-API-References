---
title: "Range"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta un intervallo di celle all'interno di un foglio di calcolo."
type: docs
url: /it/java/com.aspose.cells/range/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Range implements Iterable
```

Incapsula l'oggetto che rappresenta un intervallo di celle all'interno di un foglio di calcolo.

**Remarks**

La classe Range denota una regione di un foglio di calcolo Excel. Con questa, puoi formattare e impostare il valore dell'intervallo. E puoi anche copiare semplicemente l'intervallo di Excel.

**Example**

Il seguente esempio mostra come creare un intervallo e impostare il valore dell'intervallo di Excel.

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         // Create a range (A1:D3).
         Range range = cells.createRange("A1", "D3");
         // Set value to the range.
         range.setValue("Hello");
         //Save the Excel file
         workbook.save("book1.xlsm");
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Range(CellArea ca, Cells cells)](#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-) | Costruttore della classe. |
| [Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)](#Range-int-int-int-int-com.aspose.cells.Cells-) | Costruttore della classe. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addHyperlink(String address, String textToDisplay, String screenTip)](#addHyperlink-java.lang.String-java.lang.String-java.lang.String-) | Aggiunge un hyperlink a una cella specificata o a un intervallo di celle. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applica formati a un intervallo intero. |
| [autoFill(Range target)](#autoFill-com.aspose.cells.Range-) | Riempie automaticamente l'intervallo di destinazione. |
| [autoFill(Range target, int autoFillType)](#autoFill-com.aspose.cells.Range-int-) | Riempie automaticamente l'intervallo di destinazione. |
| [clear()](#clear--) | Cancella questo intervallo. |
| [clearComments()](#clearComments--) | Cancella i commenti di questo intervallo. |
| [clearContents()](#clearContents--) | Cancella il contenuto di questo intervallo. |
| [clearFormats()](#clearFormats--) | Cancella i formati di questo intervallo. |
| [clearHyperlinks(boolean clearFormat)](#clearHyperlinks-boolean-) | Rimuove solo i collegamenti ipertestuali. |
| [copy(Range range)](#copy-com.aspose.cells.Range-) | Copia i dati (incluse le formule), la formattazione, gli oggetti di disegno ecc. da un intervallo di origine. |
| [copy(Range range, PasteOptions options)](#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-) | Copia l'intervallo con le opzioni incolla speciale. |
| [copyData(Range range)](#copyData-com.aspose.cells.Range-) | Copia i dati delle celle (incluse le formule) da un intervallo di origine. |
| [copyStyle(Range range)](#copyStyle-com.aspose.cells.Range-) | Copia le impostazioni di stile da un intervallo di origine. |
| [copyValue(Range range)](#copyValue-com.aspose.cells.Range-) | Copia il valore della cella da un intervallo di origine. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowOffset, int columnOffset)](#get-int-int-) | Ottiene l'oggetto [Cell](../../com.aspose.cells/cell) in questo intervallo. |
| [getAddress()](#getAddress--) | Ottiene l'indirizzo dell'intervallo. |
| [getCellOrNull(int rowOffset, int columnOffset)](#getCellOrNull-int-int-) | Ottiene l'oggetto [Cell](../../com.aspose.cells/cell) o null in questo intervallo. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Ottiene il conteggio delle colonne nell'intervallo. |
| [getColumnWidth()](#getColumnWidth--) | Imposta o ottiene la larghezza della colonna di questo intervallo |
| [getCurrentRegion()](#getCurrentRegion--) | Restituisce un oggetto Range che rappresenta la regione corrente. |
| [getEntireColumn()](#getEntireColumn--) | Ottiene un oggetto Range che rappresenta l'intera colonna (o le colonne) che contiene l'intervallo specificato. |
| [getEntireRow()](#getEntireRow--) | Ottiene un oggetto Range che rappresenta l'intera riga (o le righe) che contiene l'intervallo specificato. |
| [getFirstColumn()](#getFirstColumn--) | Ottiene l'indice della prima colonna dell'intervallo. |
| [getFirstRow()](#getFirstRow--) | Ottiene l'indice della prima riga dell'intervallo. |
| [getHeight()](#getHeight--) | Ottiene la larghezza di un intervallo in punti. |
| [getHyperlinks()](#getHyperlinks--) | Ottiene tutti i collegamenti ipertestuali nell'intervallo. |
| [getLeft()](#getLeft--) | Ottiene la distanza, in punti, dal bordo sinistro della colonna A al bordo sinistro dell'intervallo. |
| [getName()](#getName--) | Ottiene il nome dell'intervallo. |
| [getOffset(int rowOffset, int columnOffset)](#getOffset-int-int-) | Ottiene l'intervallo [Range](../../com.aspose.cells/range) per offset. |
| [getRefersTo()](#getRefersTo--) | Ottiene a cosa si riferisce l'intervallo. |
| [getRowCount()](#getRowCount--) | Ottiene il conteggio delle righe nell'intervallo. |
| [getRowHeight()](#getRowHeight--) | Imposta o ottiene l'altezza delle righe in questo intervallo |
| [getTop()](#getTop--) | Ottiene la distanza, in punti, dal bordo superiore della riga 1 al bordo superiore dell'intervallo. |
| [getValue()](#getValue--) | Ottiene il valore dell'intervallo. |
| [getWidth()](#getWidth--) | Ottiene la larghezza di un intervallo in punti. |
| [getWorksheet()](#getWorksheet--) | Ottiene l'oggetto [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) che contiene questo intervallo. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range range)](#intersect-com.aspose.cells.Range-) | Restituisce un oggetto [Range](../../com.aspose.cells/range) che rappresenta l'intersezione rettangolare di due intervalli. |
| [isBlank()](#isBlank--) | Indica se l'intervallo contiene valori. |
| [isIntersect(Range range)](#isIntersect-com.aspose.cells.Range-) | Indica se l'intervallo si interseca. |
| [iterator()](#iterator--) | Ottiene l'enumeratore per le celle in questo Intervallo. |
| [merge()](#merge--) | Combina un intervallo di celle in un'unica cella. |
| [moveTo(int destRow, int destColumn)](#moveTo-int-int-) | Sposta l'intervallo corrente nell'intervallo di destinazione. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Inserisce un valore nell'intervallo; se opportuno il valore verrà convertito in un altro tipo di dato e il formato numerico della cella verrà ripristinato. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Imposta o ottiene la larghezza della colonna di questo intervallo |
| [setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)](#setInsideBorders-int-int-com.aspose.cells.CellsColor-) | Imposta i bordi interni dell'intervallo. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome dell'intervallo. |
| [setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)](#setOutlineBorder-int-int-com.aspose.cells.CellsColor-) | Imposta il bordo di contorno attorno a un intervallo di celle. |
| [setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)](#setOutlineBorder-int-int-com.aspose.cells.Color-) | Imposta il bordo di contorno attorno a un intervallo di celle. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | Imposta i bordi di contorno attorno a un intervallo di celle con lo stesso stile e colore del bordo. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Imposta i bordi di contorno attorno a un intervallo di celle con lo stesso stile e colore del bordo. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Imposta i bordi di contorno attorno a un intervallo di celle. |
| [setRowHeight(double value)](#setRowHeight-double-) | Imposta o ottiene l'altezza delle righe in questo intervallo |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Imposta lo stile dell'intervallo. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Applica lo stile della cella. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Imposta il valore dell'intervallo. |
| [toHtml(HtmlSaveOptions saveOptions)](#toHtml-com.aspose.cells.HtmlSaveOptions-) | Converti l'intervallo in HTML. |
| [toImage(ImageOrPrintOptions options)](#toImage-com.aspose.cells.ImageOrPrintOptions-) | Converte l'intervallo in immagine. |
| [toJson(JsonSaveOptions options)](#toJson-com.aspose.cells.JsonSaveOptions-) | Converti l'intervallo in valore JSON. |
| [toString()](#toString--) | Restituisce una stringa che rappresenta l'oggetto Range corrente. |
| [transpose()](#transpose--) | Trasponi (ruota) i dati da righe a colonne o viceversa. |
| [unMerge()](#unMerge--) | Separa le celle unite di questo intervallo. |
| [union(Range range)](#union-com.aspose.cells.Range-) | Restituisce l'unione di due intervalli. |
| [unionRang(Range range)](#unionRang-com.aspose.cells.Range-) | Restituisce il risultato dell'unione di due intervalli. |
| [unionRanges(Range[] ranges)](#unionRanges-com.aspose.cells.Range---) | Restituisce il risultato dell'unione di due intervalli. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Range(CellArea ca, Cells cells) {#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-}
```
public Range(CellArea ca, Cells cells)
```


Costruttore della classe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | L'intervallo. |
| cells | [Cells](../../com.aspose.cells/cells) |  |

### Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells) {#Range-int-int-int-int-com.aspose.cells.Cells-}
```
public Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)
```


Costruttore della classe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Prima riga di questo intervallo(basato su zero) |
| firstColumn | int | Prima colonna di questo intervallo (indice zero). |
| rowNumber | int | Numero di righe(basato su uno) |
| columnNumber | int | Numero di colonne (basato su 1) |
| cells | [Cells](../../com.aspose.cells/cells) | L'oggetto Range appartiene a questo oggetto Cells. |

### addHyperlink(String address, String textToDisplay, String screenTip) {#addHyperlink-java.lang.String-java.lang.String-java.lang.String-}
```
public Hyperlink addHyperlink(String address, String textToDisplay, String screenTip)
```


Aggiunge un hyperlink a una cella specificata o a un intervallo di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indirizzo | java.lang.String | Indirizzo del collegamento ipertestuale. |
| textToDisplay | java.lang.String | Il testo da visualizzare per il collegamento ipertestuale specificato. |
| screenTip | java.lang.String | Il testo screenTip per il collegamento ipertestuale specificato. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - [Hyperlink](../../com.aspose.cells/hyperlink) object.
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Applica formati a un intervallo intero.

**Remarks**

Ogni cella in questo intervallo conterrà un oggetto [Style](../../com.aspose.cells/style). Pertanto questo è un metodo che consuma molta memoria. Si prega di usarlo con attenzione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | L'oggetto stile che verrà applicato. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flag che indicano le proprietà di formattazione applicate. |

### autoFill(Range target) {#autoFill-com.aspose.cells.Range-}
```
public void autoFill(Range target)
```


Riempie automaticamente l'intervallo di destinazione.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").putValue(1);
         cells.get("A2").putValue(2);
         Range source = cells.createRange("A1:A2");
         Range target = cells.createRange("A3:A10");
         //fill 3,4,5....10 to the range A3:A10
         source.autoFill(target);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | l'intervallo di destinazione. |

### autoFill(Range target, int autoFillType) {#autoFill-com.aspose.cells.Range-int-}
```
public void autoFill(Range target, int autoFillType)
```


Riempie automaticamente l'intervallo di destinazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | L'intervallo di destinazione. |
| autoFillType | int | [AutoFillType](../../com.aspose.cells/autofilltype). Il tipo di riempimento automatico. |

### clear() {#clear--}
```
public void clear()
```


Cancella questo intervallo.

### clearComments() {#clearComments--}
```
public void clearComments()
```


Cancella i commenti di questo intervallo.

### clearContents() {#clearContents--}
```
public void clearContents()
```


Cancella il contenuto di questo intervallo.

### clearFormats() {#clearFormats--}
```
public void clearFormats()
```


Cancella i formati di questo intervallo.

### clearHyperlinks(boolean clearFormat) {#clearHyperlinks-boolean-}
```
public void clearHyperlinks(boolean clearFormat)
```


Rimuove solo i collegamenti ipertestuali.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| clearFormat | boolean | Indica se cancellare il formato dei collegamenti ipertestuali. |

### copy(Range range) {#copy-com.aspose.cells.Range-}
```
public void copy(Range range)
```


Copia i dati (incluse le formule), la formattazione, gli oggetti di disegno ecc. da un intervallo di origine.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         Range range1 = cells.createRange("A1:A5");
         Range range2 = cells.createRange("A6:A10");
         //Copy the range.
         range1.copy(range2);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Oggetto [Range](../../com.aspose.cells/range) di origine. |

### copy(Range range, PasteOptions options) {#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-}
```
public void copy(Range range, PasteOptions options)
```


Copia l'intervallo con le opzioni incolla speciale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | L'intervallo di origine. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | Le opzioni di incolla speciale. |

### copyData(Range range) {#copyData-com.aspose.cells.Range-}
```
public void copyData(Range range)
```


Copia i dati delle celle (incluse le formule) da un intervallo di origine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Oggetto [Range](../../com.aspose.cells/range) di origine. |

### copyStyle(Range range) {#copyStyle-com.aspose.cells.Range-}
```
public void copyStyle(Range range)
```


Copia le impostazioni di stile da un intervallo di origine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Oggetto [Range](../../com.aspose.cells/range) di origine. |

### copyValue(Range range) {#copyValue-com.aspose.cells.Range-}
```
public void copyValue(Range range)
```


Copia il valore della cella da un intervallo di origine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Oggetto [Range](../../com.aspose.cells/range) di origine. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int rowOffset, int columnOffset) {#get-int-int-}
```
public Cell get(int rowOffset, int columnOffset)
```


Ottiene l'oggetto [Cell](../../com.aspose.cells/cell) in questo intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | int | Scostamento di riga in questo intervallo, basato su zero. |
| columnOffset | int | Scostamento di colonna in questo intervallo, basato su zero. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getAddress() {#getAddress--}
```
public String getAddress()
```


Ottiene l'indirizzo dell'intervallo.

**Returns:**
java.lang.String
### getCellOrNull(int rowOffset, int columnOffset) {#getCellOrNull-int-int-}
```
public Cell getCellOrNull(int rowOffset, int columnOffset)
```


Ottiene l'oggetto [Cell](../../com.aspose.cells/cell) o null in questo intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | int | Scostamento di riga in questo intervallo, basato su zero. |
| columnOffset | int | Scostamento di colonna in questo intervallo, basato su zero. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Ottiene il conteggio delle colonne nell'intervallo.

**Returns:**
int
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


Imposta o ottiene la larghezza della colonna di questo intervallo

**Returns:**
double
### getCurrentRegion() {#getCurrentRegion--}
```
public Range getCurrentRegion()
```


Restituisce un oggetto Range che rappresenta la regione corrente. La regione corrente è un intervallo delimitato da qualsiasi combinazione di righe vuote e colonne vuote.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireColumn() {#getEntireColumn--}
```
public Range getEntireColumn()
```


Ottiene un oggetto Range che rappresenta l'intera colonna (o le colonne) che contiene l'intervallo specificato.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireRow() {#getEntireRow--}
```
public Range getEntireRow()
```


Ottiene un oggetto Range che rappresenta l'intera riga (o le righe) che contiene l'intervallo specificato.

**Returns:**
[Range](../../com.aspose.cells/range)
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


Ottiene l'indice della prima colonna dell'intervallo.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


Ottiene l'indice della prima riga dell'intervallo.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Ottiene la larghezza di un intervallo in punti.

**Returns:**
double
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


Ottiene tutti i collegamenti ipertestuali nell'intervallo.

**Returns:**
com.aspose.cells.Hyperlink[]
### getLeft() {#getLeft--}
```
public double getLeft()
```


Ottiene la distanza, in punti, dal bordo sinistro della colonna A al bordo sinistro dell'intervallo.

**Returns:**
double
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome dell'intervallo.

**Remarks**

L'intervallo denominato è supportato. Per esempio,

range.Name = "Sheet1!MyRange";

**Returns:**
java.lang.String
### getOffset(int rowOffset, int columnOffset) {#getOffset-int-int-}
```
public Range getOffset(int rowOffset, int columnOffset)
```


Ottiene l'intervallo [Range](../../com.aspose.cells/range) per offset.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | int | Scostamento di riga in questo intervallo, basato su zero. |
| columnOffset | int | Scostamento di colonna in questo intervallo, basato su zero. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Ottiene a cosa si riferisce l'intervallo.

**Returns:**
java.lang.String
### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Ottiene il conteggio delle righe nell'intervallo.

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


Imposta o ottiene l'altezza delle righe in questo intervallo

**Returns:**
double
### getTop() {#getTop--}
```
public double getTop()
```


Ottiene la distanza, in punti, dal bordo superiore della riga 1 al bordo superiore dell'intervallo.

**Returns:**
double
### getValue() {#getValue--}
```
public Object getValue()
```


Ottiene il valore dell'intervallo.

**Remarks**

Se l'intervallo contiene più celle, l'oggetto restituito/applicato dovrebbe essere Object[][].

**Returns:**
java.lang.Object
### getWidth() {#getWidth--}
```
public double getWidth()
```


Ottiene la larghezza di un intervallo in punti.

**Returns:**
double
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Ottiene l'oggetto [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) che contiene questo intervallo.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range range) {#intersect-com.aspose.cells.Range-}
```
public Range intersect(Range range)
```


Restituisce un oggetto [Range](../../com.aspose.cells/range) che rappresenta l'intersezione rettangolare di due intervalli.

**Remarks**

Se i due intervalli non si intersecano, restituisce null.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         Range range1 = cells.createRange("A1:A5");
         Range range2 = cells.createRange("A3:A10");
         //Get intersected range of the two ranges.
         Range intersectRange = range1.intersect(range2);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | L'intervallo di intersezione. |

**Returns:**
[Range](../../com.aspose.cells/range) - Returns a [Range](../../com.aspose.cells/range) object
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Indica se l'intervallo contiene valori.

**Returns:**
boolean -
### isIntersect(Range range) {#isIntersect-com.aspose.cells.Range-}
```
public boolean isIntersect(Range range)
```


Indica se l'intervallo si interseca.

**Remarks**

Se i due intervalli non sono nello stesso foglio di lavoro, restituisce false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | L'intervallo. |

**Returns:**
boolean - Indica se l'intervallo si interseca.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Ottiene l'enumeratore per le celle in questo Intervallo.

**Remarks**

Durante l'attraversamento degli elementi tramite l'Enumerator restituito, la collezione di celle non dovrebbe essere modificata (ad esempio operazioni che creano nuove Cell/Row o eliminano celle/righe esistenti). Altrimenti l'enumeratore potrebbe non riuscire a attraversare correttamente tutte le celle (alcuni elementi potrebbero essere attraversati più volte o saltati).

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.createRange("B2:C3").iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - L'enumeratore delle celle
### merge() {#merge--}
```
public void merge()
```


Combina un intervallo di celle in un'unica cella.

**Remarks**

Fai riferimento alla cella unita tramite l'indirizzo della cella in alto a sinistra nell'intervallo.

### moveTo(int destRow, int destColumn) {#moveTo-int-int-}
```
public void moveTo(int destRow, int destColumn)
```


Sposta l'intervallo corrente nell'intervallo di destinazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destRow | int | La riga iniziale dell'intervallo di destinazione. |
| destColumn | int | La colonna iniziale dell'intervallo di destinazione. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Inserisce un valore nell'intervallo; se opportuno il valore verrà convertito in un altro tipo di dato e il formato numerico della cella verrà ripristinato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringValue | java.lang.String | Valore di input |
| isConverted | boolean | True: convertito in un altro tipo di dato se appropriato. |
| setStyle | boolean | True: imposta il formato numerico nello stile della cella durante la conversione in un altro tipo di dato |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


Imposta o ottiene la larghezza della colonna di questo intervallo

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor) {#setInsideBorders-int-int-com.aspose.cells.CellsColor-}
```
public void setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)
```


Imposta i bordi interni dell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). All'interno del tipo di bordo, può essere solo [BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) e [BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL). |
| lineStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Lo stile del bordo. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Il colore del bordo. |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Imposta il nome dell'intervallo.

**Remarks**

L'intervallo denominato è supportato. Per esempio,

range.Name = "Sheet1!MyRange";

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor) {#setOutlineBorder-int-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)
```


Imposta il bordo di contorno attorno a un intervallo di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Lato del bordo. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Stile del bordo. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Colore del bordo. |

### setOutlineBorder(int borderEdge, int borderStyle, Color borderColor) {#setOutlineBorder-int-int-com.aspose.cells.Color-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)
```


Imposta il bordo di contorno attorno a un intervallo di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Lato del bordo. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Stile del bordo. |
| borderColor | [Color](../../com.aspose.cells/color) | Colore del bordo. |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


Imposta i bordi di contorno attorno a un intervallo di celle con lo stesso stile e colore del bordo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Stile del bordo. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Colore del bordo. |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Imposta i bordi di contorno attorno a un intervallo di celle con lo stesso stile e colore del bordo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Stile del bordo. |
| borderColor | [Color](../../com.aspose.cells/color) | Colore del bordo. |

### setOutlineBorders(int[] borderStyles, Color[] borderColors) {#setOutlineBorders-int---com.aspose.cells.Color---}
```
public void setOutlineBorders(int[] borderStyles, Color[] borderColors)
```


Imposta i bordi di contorno attorno a un intervallo di celle.

**Remarks**

Sia la lunghezza di borderStyles che quella di borderStyles deve essere 4. L'ordine di borderStyles e borderStyles deve essere top,bottom,left,right.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderStyles | int[] | [CellBorderType](../../com.aspose.cells/cellbordertype). Stili del bordo. |
| borderColors | [Color\[\]](../../com.aspose.cells/color) | Colori dei bordi. |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


Imposta o ottiene l'altezza delle righe in questo intervallo

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Imposta lo stile dell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | L'oggetto Style. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


Applica lo stile della cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Lo stile della cella. |
| explicitFlag | boolean | True, sovrascrive solo la formattazione che è impostata esplicitamente. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Imposta il valore dell'intervallo.

**Remarks**

Se l'intervallo contiene più celle, l'oggetto restituito/applicato dovrebbe essere Object[][].

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

### toHtml(HtmlSaveOptions saveOptions) {#toHtml-com.aspose.cells.HtmlSaveOptions-}
```
public byte[] toHtml(HtmlSaveOptions saveOptions)
```


Converti l'intervallo in HTML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveOptions | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) | Opzioni per la conversione dell'intervallo in html. |

**Returns:**
byte[] -
### toImage(ImageOrPrintOptions options) {#toImage-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(ImageOrPrintOptions options)
```


Converte l'intervallo in immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Le opzioni per convertire questo intervallo in immagine |

**Returns:**
byte[] -
### toJson(JsonSaveOptions options) {#toJson-com.aspose.cells.JsonSaveOptions-}
```
public String toJson(JsonSaveOptions options)
```


Converti l'intervallo in valore JSON.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | Le opzioni di conversione |

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


Restituisce una stringa che rappresenta l'oggetto Range corrente.

**Returns:**
java.lang.String -
### transpose() {#transpose--}
```
public void transpose()
```


Trasponi (ruota) i dati da righe a colonne o viceversa.

### unMerge() {#unMerge--}
```
public void unMerge()
```


Separa le celle unite di questo intervallo.

### union(Range range) {#union-com.aspose.cells.Range-}
```
public ArrayList union(Range range)
```


Restituisce l'unione di due intervalli.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Range.UnionRanges(). Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2023. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | L'intervallo |

**Returns:**
java.util.ArrayList - L'unione di due intervalli.
### unionRang(Range range) {#unionRang-com.aspose.cells.Range-}
```
public Range[] unionRang(Range range)
```


Restituisce il risultato dell'unione di due intervalli.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Range.UnionRanges(). Questo metodo sarà rimosso 12 mesi dopo, a partire da maggio 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | L'intervallo |

**Returns:**
com.aspose.cells.Range[] - L'unione di due intervalli.
### unionRanges(Range[] ranges) {#unionRanges-com.aspose.cells.Range---}
```
public UnionRange unionRanges(Range[] ranges)
```


Restituisce il risultato dell'unione di due intervalli.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | L'intervallo |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - The union of two ranges.
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

