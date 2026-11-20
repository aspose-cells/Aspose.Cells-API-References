---
title: "Riga"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta una singola riga in un foglio di lavoro."
type: docs
url: /it/java/com.aspose.cells/row/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Row implements Iterable
```

Rappresenta una singola riga in un foglio di lavoro.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setBackgroundColor(Color.getBlue());
 
         //Setting the foreground color to Red
         style.setForegroundColor(Color.getRed());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.DIAGONAL_STRIPE);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
          //Apply Style to first row
         row.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applica formati per un'intera riga. |
| [copySettings(Row source, boolean checkStyle)](#copySettings-com.aspose.cells.Row-boolean-) | Copia le impostazioni della riga, come stile, altezza, visibilità, ...ecc. |
| [equals(Row row)](#equals-com.aspose.cells.Row-) | Verifica se questo oggetto si riferisce alla stessa riga di un altro oggetto riga. |
| [equals(Object obj)](#equals-java.lang.Object-) | Verifica se questo oggetto si riferisce alla stessa riga di un altro. |
| [get(int column)](#get-int-) | Ottiene la cella. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Ottieni la cella tramite indice specifico nella collezione di celle di questa riga. |
| [getCellOrNull(int column)](#getCellOrNull-int-) | Ottiene la cella o null nell'indice specifico. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Ottiene il primo oggetto cella nella riga. |
| [getFirstDataCell()](#getFirstDataCell--) | Ottiene la prima cella non vuota nella riga. |
| [getGroupLevel()](#getGroupLevel--) | Ottiene il livello di gruppo della riga. |
| [getHeight()](#getHeight--) | Ottiene l'altezza della riga in unità di punti. |
| [getIndex()](#getIndex--) | Ottiene l'indice di questa riga. |
| [getLastCell()](#getLastCell--) | Ottiene l'ultimo oggetto cella nella riga. |
| [getLastDataCell()](#getLastDataCell--) | Ottiene l'ultima cella non vuota nella riga. |
| [getStyle()](#getStyle--) | Ottiene lo stile di questa riga. |
| [hasCustomStyle()](#hasCustomStyle--) | Indica se questa riga ha impostazioni di stile personalizzate (diverse da quelle predefinite ereditate dalla cartella di lavoro). |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Indica se la riga contiene dati |
| [isCollapsed()](#isCollapsed--) | se la riga è compressa |
| [isHeightMatched()](#isHeightMatched--) | Indica se l'altezza della riga corrisponde all'impostazione corrente del carattere predefinito della cartella di lavoro. |
| [isHidden()](#isHidden--) | Indica se la riga è nascosta. |
| [iterator()](#iterator--) | Ottiene l'enumeratore delle celle |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Ottiene un enumeratore che itera le celle attraverso questa riga. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | se la riga è compressa |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Ottiene il livello di gruppo della riga. |
| [setHeight(double value)](#setHeight-double-) | Imposta l'altezza della riga in unità di punti. |
| [setHeightMatched(boolean value)](#setHeightMatched-boolean-) | Indica se l'altezza della riga corrisponde all'impostazione corrente del carattere predefinito della cartella di lavoro. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indica se la riga è nascosta. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Imposta lo stile di questa riga. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Applica formati per un'intera riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | L'oggetto stile che verrà applicato. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flag che indicano le proprietà di formattazione applicate. |

### copySettings(Row source, boolean checkStyle) {#copySettings-com.aspose.cells.Row-boolean-}
```
public void copySettings(Row source, boolean checkStyle)
```


Copia le impostazioni della riga, come stile, altezza, visibilità, ...ecc.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | [Row](../../com.aspose.cells/row) | la riga sorgente le cui impostazioni saranno copiate in questa |
| checkStyle | boolean | se controllare e raccogliere lo stile. Ha effetto solo e è necessario quando due oggetti riga appartengono a cartelle di lavoro diverse e gli stili delle due cartelle di lavoro sono diversi. |

### equals(Row row) {#equals-com.aspose.cells.Row-}
```
public boolean equals(Row row)
```


Verifica se questo oggetto si riferisce alla stessa riga di un altro oggetto riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | un altro oggetto riga |

**Returns:**
boolean - true se due oggetti riga si riferiscono alla stessa riga.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Verifica se questo oggetto si riferisce alla stessa riga di un altro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | un altro oggetto |

**Returns:**
boolean - true se due oggetti si riferiscono alla stessa riga.
### get(int column) {#get-int-}
```
public Cell get(int column)
```


Ottiene la cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | L'indice della colonna |

**Returns:**
[Cell](../../com.aspose.cells/cell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public Cell getCellByIndex(int index)
```


Ottieni la cella tramite indice specifico nella collezione di celle di questa riga.

**Remarks**

Per attraversare tutte le celle in sequenza senza modifiche, usare [iterator()](../../com.aspose.cells/row\#iterator--) offrirà prestazioni migliori rispetto all'utilizzo di questo metodo per ottenere le celle una alla volta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice (posizione) della cella nella collezione di celle di questa riga. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The Cell object at given position.
### getCellOrNull(int column) {#getCellOrNull-int-}
```
public Cell getCellOrNull(int column)
```


Ottiene la cella o null nell'indice specifico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | L'indice della colonna |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Returns the cell object if the cell exists. Or returns null if the cell object does not exist.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Ottiene il primo oggetto cella nella riga.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataCell() {#getFirstDataCell--}
```
public Cell getFirstDataCell()
```


Ottiene la prima cella non vuota nella riga.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Ottiene il livello di gruppo della riga.

**Returns:**
byte
### getHeight() {#getHeight--}
```
public double getHeight()
```


Ottiene l'altezza della riga in unità di punti.

**Returns:**
double
### getIndex() {#getIndex--}
```
public int getIndex()
```


Ottiene l'indice di questa riga.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Ottiene l'ultimo oggetto cella nella riga.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataCell() {#getLastDataCell--}
```
public Cell getLastDataCell()
```


Ottiene l'ultima cella non vuota nella riga.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Ottiene lo stile di questa riga.

**Remarks**

Modificare direttamente l'oggetto stile restituito non ha effetto su questa riga o su qualsiasi cella in questa riga. È necessario chiamare il metodo [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-) o [setStyle(Style)](../../com.aspose.cells/row\#setStyle-Style-) per applicare la modifica a questa riga.

Lo stile della riga è lo stile che verrà ereditato dalle celle in questa riga (quelle celle che non hanno impostazioni di stile personalizzate, come le celle esistenti che non hanno uno stile impostato esplicitamente, o quelle che non sono state istanziate).

**Returns:**
[Style](../../com.aspose.cells/style)
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Indica se questa riga ha impostazioni di stile personalizzate (diverse da quelle predefinite ereditate dalla cartella di lavoro).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Indica se la riga contiene dati

**Returns:**
boolean
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


se la riga è compressa

**Returns:**
boolean
### isHeightMatched() {#isHeightMatched--}
```
public boolean isHeightMatched()
```


Indica se l'altezza della riga corrisponde all'impostazione corrente del carattere predefinito della cartella di lavoro. Il valore true di questa proprietà indica anche che l'altezza della riga è \"automatica\" senza un valore di altezza personalizzato impostato dall'utente.

**Remarks**

Quando questa proprietà è true, se il contenuto di questa riga cambia, generalmente l'altezza della riga deve essere ricalcolata (ad esempio tramite [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)) per ottenere lo stesso risultato di quanto mostrato in MS Excel quando si apre la cartella di lavoro.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indica se la riga è nascosta.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Ottiene l'enumeratore delle celle

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().get(1).iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - L'enumeratore delle celle che attraverserà tutte le celle esistenti in questa riga.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


Ottiene un enumeratore che itera le celle attraverso questa riga.

**Remarks**

Se la riga verrà modificata (tramite operazioni che possono causare l'instanziazione di una nuova Cell o la rimozione di una Cell esistente) durante l'attraversamento con l'enumeratore, dovrebbe essere usato un enumeratore sincronizzato invece di quello normale affinché l'attraversamento possa continuare dalla posizione subito dopo quella attraversata dall'ultimo MoveNext(). Tuttavia, oltre al vantaggio che nessun elemento venga saltato o attraversato più volte, lo svantaggio dell'enumeratore sincronizzato è che le prestazioni saranno leggermente degradate rispetto all'enumeratore normale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| invertito | boolean | se enumerare le celle in ordine inverso |
| sincronizzato | boolean | se l'enumeratore restituito deve verificare la modifica delle celle in questa riga e mantenerlo sincronizzato. |

**Returns:**
java.util.Iterator - L'enumeratore delle celle che attraverserà tutte le celle esistenti in questa riga.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


se la riga è compressa

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


Ottiene il livello di gruppo della riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Imposta l'altezza della riga in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setHeightMatched(boolean value) {#setHeightMatched-boolean-}
```
public void setHeightMatched(boolean value)
```


Indica se l'altezza della riga corrisponde all'impostazione corrente del carattere predefinito della cartella di lavoro. Il valore true di questa proprietà indica anche che l'altezza della riga è \"automatica\" senza un valore di altezza personalizzato impostato dall'utente.

**Remarks**

Quando questa proprietà è true, se il contenuto di questa riga cambia, generalmente l'altezza della riga deve essere ricalcolata (ad esempio tramite [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)) per ottenere lo stesso risultato di quanto mostrato in MS Excel quando si apre la cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indica se la riga è nascosta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Imposta lo stile di questa riga.

**Remarks**

Questo metodo imposta solo lo stile fornito come stile predefinito per questa riga, senza modificare le impostazioni di stile per le celle esistenti in questa riga. Per aggiornare le impostazioni di stile delle celle esistenti allo stile specificato allo stesso tempo, utilizzare [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | lo stile da utilizzare come stile predefinito per le celle in questa riga. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
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

