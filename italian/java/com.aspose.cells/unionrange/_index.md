---
title: "UnionRange"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un intervallo di unione."
type: docs
url: /it/java/com.aspose.cells/unionrange/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class UnionRange implements Iterable
```

Rappresenta un intervallo di unione.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applica formati a un intervallo intero. |
| [copy(UnionRange range, PasteOptions options)](#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-) | Copia l'intervallo con le opzioni incolla speciale. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellCount()](#getCellCount--) | Ottiene il conteggio di tutte le celle nell'intervallo. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Ottiene il conteggio delle righe nell'intervallo. |
| [getFirstColumn()](#getFirstColumn--) | Ottiene l'indice della prima colonna dell'intervallo. |
| [getFirstRow()](#getFirstRow--) | Ottiene l'indice della prima riga dell'intervallo. |
| [getHyperlinks()](#getHyperlinks--) | Ottiene tutti i collegamenti ipertestuali nell'intervallo. |
| [getName()](#getName--) | Ottiene il nome dell'intervallo. |
| [getRangeCount()](#getRangeCount--) | Ottiene il conteggio degli intervalli. |
| [getRanges()](#getRanges--) | Ottiene tutti gli intervalli di unione. |
| [getRefersTo()](#getRefersTo--) | Ottiene a cosa si riferisce l'intervallo. |
| [getRowCount()](#getRowCount--) | Ottiene il conteggio delle righe nell'intervallo. |
| [getValue()](#getValue--) | Ottiene i valori dell'intervallo. |
| [hasRange()](#hasRange--) | Indica se questo ha un intervallo. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range[] ranges)](#intersect-com.aspose.cells.Range---) | Interseca un altro intervallo. |
| [intersect(UnionRange unionRange)](#intersect-com.aspose.cells.UnionRange-) | Interseca un altro intervallo. |
| [intersect(String range)](#intersect-java.lang.String-) | Interseca un altro intervallo. |
| [iterator()](#iterator--) | Ottiene l'enumeratore per le celle in questo Intervallo. |
| [merge()](#merge--) | Combina un intervallo di celle in un'unica cella. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Inserisce un valore nell'intervallo; se opportuno il valore verrà convertito in un altro tipo di dato e il formato numerico della cella verrà ripristinato. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome dell'intervallo. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Imposta i bordi di contorno attorno a un intervallo di celle con lo stesso stile e colore del bordo. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Imposta i bordi di contorno attorno a un intervallo di celle. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Imposta lo stile dell'intervallo. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Imposta i valori dell'intervallo. |
| [toString()](#toString--) |  |
| [unMerge()](#unMerge--) | Separa le celle unite di questo intervallo. |
| [union(Range[] ranges)](#union-com.aspose.cells.Range---) | Unisci gli intervalli. |
| [union(UnionRange unionRange)](#union-com.aspose.cells.UnionRange-) | Unisci un altro intervallo. |
| [union(String range)](#union-java.lang.String-) | Unisci un altro intervallo. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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

### copy(UnionRange range, PasteOptions options) {#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-}
```
public void copy(UnionRange range, PasteOptions options)
```


Copia l'intervallo con le opzioni incolla speciale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [UnionRange](../../com.aspose.cells/unionrange) | L'intervallo di origine. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | Le opzioni di incolla speciale. |

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
### getCellCount() {#getCellCount--}
```
public int getCellCount()
```


Ottiene il conteggio di tutte le celle nell'intervallo.

**Returns:**
int
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


Ottiene il conteggio delle righe nell'intervallo.

**Remarks**

Ha effetto solo quando contiene un solo intervallo.

**Returns:**
int
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


Ottiene l'indice della prima colonna dell'intervallo.

**Remarks**

Ha effetto solo quando contiene un solo intervallo.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


Ottiene l'indice della prima riga dell'intervallo.

**Remarks**

Ha effetto solo quando contiene un solo intervallo.

**Returns:**
int
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


Ottiene tutti i collegamenti ipertestuali nell'intervallo.

**Returns:**
com.aspose.cells.Hyperlink[]
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
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


Ottiene il conteggio degli intervalli.

**Returns:**
int
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


Ottiene tutti gli intervalli di unione.

**Returns:**
com.aspose.cells.Range[]
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

**Remarks**

Ha effetto solo quando contiene un solo intervallo.

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Ottiene i valori dell'intervallo.

**Returns:**
java.lang.Object
### hasRange() {#hasRange--}
```
public boolean hasRange()
```


Indica se questo ha un intervallo.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range[] ranges) {#intersect-com.aspose.cells.Range---}
```
public UnionRange intersect(Range[] ranges)
```


Interseca un altro intervallo.

**Remarks**

Se i due intervalli di unione non si intersecano, restituisce null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | L'intervallo. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(UnionRange unionRange) {#intersect-com.aspose.cells.UnionRange-}
```
public UnionRange intersect(UnionRange unionRange)
```


Interseca un altro intervallo.

**Remarks**

Se i due intervalli di unione non si intersecano, restituisce null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | L'intervallo. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(String range) {#intersect-java.lang.String-}
```
public UnionRange intersect(String range)
```


Interseca un altro intervallo.

**Remarks**

Se i due intervalli di unione non si intersecano, restituisce null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | java.lang.String | L'intervallo. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### iterator() {#iterator--}
```
public Iterator iterator()
```


Ottiene l'enumeratore per le celle in questo Intervallo.

**Remarks**

Durante l'attraversamento degli elementi tramite l'Enumerator restituito, la collezione di celle non dovrebbe essere modificata (ad esempio operazioni che creano nuove Cell/Row o eliminano celle/righe esistenti). Altrimenti l'enumeratore potrebbe non riuscire a attraversare correttamente tutte le celle (alcuni elementi potrebbero essere attraversati più volte o saltati).

**Returns:**
java.util.Iterator - L'enumeratore delle celle
### merge() {#merge--}
```
public void merge()
```


Combina un intervallo di celle in un'unica cella.

**Remarks**

Fai riferimento alla cella unita tramite l'indirizzo della cella in alto a sinistra nell'intervallo.

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

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Imposta lo stile dell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | L'oggetto Style. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Imposta i valori dell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unMerge() {#unMerge--}
```
public void unMerge()
```


Separa le celle unite di questo intervallo.

### union(Range[] ranges) {#union-com.aspose.cells.Range---}
```
public UnionRange union(Range[] ranges)
```


Unisci gli intervalli.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | Gli intervalli. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(UnionRange unionRange) {#union-com.aspose.cells.UnionRange-}
```
public UnionRange union(UnionRange unionRange)
```


Unisci un altro intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | L'intervallo. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(String range) {#union-java.lang.String-}
```
public UnionRange union(String range)
```


Unisci un altro intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | java.lang.String | L'intervallo. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
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

