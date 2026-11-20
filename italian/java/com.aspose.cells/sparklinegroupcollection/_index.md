---
title: "SparklineGroupCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula una raccolta di oggetti."
type: docs
url: /it/java/com.aspose.cells/sparklinegroupcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SparklineGroupCollection extends CollectionBase
```

Incapsula una raccolta di oggetti [SparklineGroup](../../com.aspose.cells/sparklinegroup).

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
 
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, "A1:D1", false, ca);
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         book.save("output.xlsx", SaveFormat.XLSX);
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(int type)](#add-int-) | Aggiunge un [SparklineGroup](../../com.aspose.cells/sparklinegroup) con uno [Sparkline](../../com.aspose.cells/sparkline) alla raccolta. |
| [add(int type, String dataRange, boolean isVertical, CellArea locationRange)](#add-int-java.lang.String-boolean-com.aspose.cells.CellArea-) | Aggiunge un [SparklineGroup](../../com.aspose.cells/sparklinegroup) con alcuni [Sparkline](../../com.aspose.cells/sparkline) alla raccolta. |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [clear()](#clear--) | Rimuove tutti gli oggetti dall'istanza di CollectionBase. |
| [clearSparklineGroups(CellArea cellArea)](#clearSparklineGroups-com.aspose.cells.CellArea-) | Cancella i gruppi di sparkline che si sovrappongono a un'area di celle. |
| [clearSparklines(CellArea cellArea)](#clearSparklines-com.aspose.cells.CellArea-) | Cancella le sparkline che si trovano all'interno di un'area di celle. |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene l'elemento [SparklineGroup](../../com.aspose.cells/sparklinegroup) all'indice specificato. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Rimuove l'elemento all'indice specificato. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int type) {#add-int-}
```
public int add(int type)
```


Aggiunge un [SparklineGroup](../../com.aspose.cells/sparklinegroup) con uno [Sparkline](../../com.aspose.cells/sparkline) alla raccolta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [SparklineType](../../com.aspose.cells/sparklinetype). Specifica il tipo del gruppo Sparkline. |

**Returns:**
int - indice dell'oggetto [SparklineGroup](../../com.aspose.cells/sparklinegroup).
### add(int type, String dataRange, boolean isVertical, CellArea locationRange) {#add-int-java.lang.String-boolean-com.aspose.cells.CellArea-}
```
public int add(int type, String dataRange, boolean isVertical, CellArea locationRange)
```


Aggiunge un [SparklineGroup](../../com.aspose.cells/sparklinegroup) con alcuni [Sparkline](../../com.aspose.cells/sparkline) alla raccolta.

**Remarks**

Questo metodo creerà anche le sparkline. Se è true, il numero di righe in dataRange e locationRange deve essere lo stesso. Se è false, il numero di colonne in dataRange e locationRange deve essere lo stesso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [SparklineType](../../com.aspose.cells/sparklinetype). Specifica il tipo del gruppo Sparkline. |
| dataRange | java.lang.String | Specifica l'intervallo di dati del gruppo sparkline. |
| isVertical | boolean | Specifica se tracciare le sparkline dall'intervallo di dati per riga o per colonna. |
| locationRange | [CellArea](../../com.aspose.cells/cellarea) | Specifica dove posizionare gli sparklines. |

**Returns:**
int - indice dell'oggetto [SparklineGroup](../../com.aspose.cells/sparklinegroup).
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Aggiunge un elemento all'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | L'Object da aggiungere all'istanza di CollectionBase. |

**Returns:**
int - La posizione in cui è stato inserito il nuovo elemento.
### clear() {#clear--}
```
public void clear()
```


Rimuove tutti gli oggetti dall'istanza di CollectionBase.

### clearSparklineGroups(CellArea cellArea) {#clearSparklineGroups-com.aspose.cells.CellArea-}
```
public void clearSparklineGroups(CellArea cellArea)
```


Cancella i gruppi di sparkline che si sovrappongono a un'area di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Specifica l'area di celle |

### clearSparklines(CellArea cellArea) {#clearSparklines-com.aspose.cells.CellArea-}
```
public void clearSparklines(CellArea cellArea)
```


Cancella le sparkline che si trovano all'interno di un'area di celle.

**Remarks**

[SparklineGroup](../../com.aspose.cells/sparklinegroup) will be removed too if it does not contains any [Sparkline](../../com.aspose.cells/sparkline).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Specifica l'area di celle |

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Restituisce se l'istanza contiene questo oggetto

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | oggetto di test |

**Returns:**
boolean - Se l'istanza contiene questo oggetto
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
### get(int index) {#get-int-}
```
public SparklineGroup get(int index)
```


Ottiene l'elemento [SparklineGroup](../../com.aspose.cells/sparklinegroup) all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

**Returns:**
[SparklineGroup](../../com.aspose.cells/sparklinegroup) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Ottiene il numero di elementi contenuti nell'istanza di CollectionBase.

**Returns:**
int - Il numero di elementi contenuti nell'istanza di CollectionBase.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Determina l'indice di un elemento specifico nell'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |

**Returns:**
int - L'indice del valore se trovato nella lista; altrimenti, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase.

**Returns:**
java.util.Iterator - Un iteratore per l'istanza di CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Rimuove l'elemento all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento da rimuovere. |

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

