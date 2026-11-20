---
title: "SlicerCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Specifica la raccolta di tutti gli oggetti Slicer nel foglio di lavoro specificato."
type: docs
url: /it/java/com.aspose.cells/slicercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SlicerCollection extends CollectionBase
```

Specifica la raccolta di tutti gli oggetti Slicer nel foglio di lavoro specificato.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
 
         //do your business
 
         book.save("out.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(ListObject table, ListColumn listColumn, int row, int column)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-) | Aggiungi un nuovo Slicer usando ListObjet come origine dati |
| [add(ListObject table, ListColumn listColumn, String destCellName)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-) | Aggiungi un nuovo Slicer usando ListObjet come origine dati |
| [add(ListObject table, int index, String destCellName)](#add-com.aspose.cells.ListObject-int-java.lang.String-) | Aggiungi un nuovo Slicer usando ListObjet come origine dati |
| [add(PivotTable pivot, int row, int column, PivotField baseField)](#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-) | Aggiungi un nuovo Slicer usando PivotTable come origine dati |
| [add(PivotTable pivot, int row, int column, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-int-int-int-) | Aggiungi un nuovo Slicer usando PivotTable come origine dati |
| [add(PivotTable pivot, int row, int column, String baseFieldName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Aggiungi un nuovo Slicer usando PivotTable come origine dati |
| [add(PivotTable pivot, String destCellName, PivotField baseField)](#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-) | Aggiungi un nuovo Slicer usando PivotTable come origine dati |
| [add(PivotTable pivot, String destCellName, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-java.lang.String-int-) | Aggiungi un nuovo Slicer usando PivotTable come origine dati |
| [add(PivotTable pivot, String destCellName, String baseFieldName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Aggiungi un nuovo Slicer usando PivotTable come origine dati |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [clear()](#clear--) | Cancella tutti i Slicer. |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene il Slicer per indice. |
| [get(String name)](#get-java.lang.String-) | Ottiene il Slicer per nome del slicer. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Slicer slicer)](#remove-com.aspose.cells.Slicer-) | Rimuovi lo Slicer specificato |
| [removeAt(int index)](#removeAt-int-) | Elimina lo Slicer all'indice specificato |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(ListObject table, ListColumn listColumn, int row, int column) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-}
```
public int add(ListObject table, ListColumn listColumn, int row, int column)
```


Aggiungi un nuovo Slicer usando ListObjet come origine dati

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | Oggetto ListObject |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | La ListColumn in ListObject.ListColumns |
| riga | int | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| colonna | int | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |

**Returns:**
int - Il nuovo indice di aggiunta Slicer
### add(ListObject table, ListColumn listColumn, String destCellName) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-}
```
public int add(ListObject table, ListColumn listColumn, String destCellName)
```


Aggiungi un nuovo Slicer usando ListObjet come origine dati

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | Oggetto ListObject |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | La ListColumn in ListObject.ListColumns |
| destCellName | java.lang.String | La cella nell'angolo in alto a sinistra dell'intervallo Slicer. |

**Returns:**
int - Il nuovo indice di aggiunta Slicer
### add(ListObject table, int index, String destCellName) {#add-com.aspose.cells.ListObject-int-java.lang.String-}
```
public int add(ListObject table, int index, String destCellName)
```


Aggiungi un nuovo Slicer usando ListObjet come origine dati

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | Oggetto ListObject |
| indice | int | L'indice di ListColumn in ListObject.ListColumns |
| destCellName | java.lang.String | La cella nell'angolo in alto a sinistra dell'intervallo Slicer. |

**Returns:**
int - Il nuovo indice di aggiunta Slicer
### add(PivotTable pivot, int row, int column, PivotField baseField) {#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, int row, int column, PivotField baseField)
```


Aggiungi un nuovo Slicer usando PivotTable come origine dati

**Example**

```
         slicers.add(pivot, 3, 12, pivot.getBaseFields().get(0));
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Oggetto PivotTable |
| riga | int | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| colonna | int | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | The PivotField in PivotTable.BaseFields |

**Returns:**
int - Il nuovo indice di aggiunta Slicer
### add(PivotTable pivot, int row, int column, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-int-int-int-}
```
public int add(PivotTable pivot, int row, int column, int baseFieldIndex)
```


Aggiungi un nuovo Slicer usando PivotTable come origine dati

**Example**

```
         slicers.add(pivot, 20, 8, 0);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Oggetto PivotTable |
| riga | int | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| colonna | int | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| baseFieldIndex | int | L'indice del PivotField in PivotTable.BaseFields |

**Returns:**
int - Il nuovo indice di aggiunta Slicer
### add(PivotTable pivot, int row, int column, String baseFieldName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivot, int row, int column, String baseFieldName)
```


Aggiungi un nuovo Slicer usando PivotTable come origine dati

**Example**

```
         slicers.add(pivot, 20, 12, "fruit");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Oggetto PivotTable |
| riga | int | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| colonna | int | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| baseFieldName | java.lang.String | Il nome del PivotField in PivotTable.BaseFields |

**Returns:**
int - Il nuovo indice di aggiunta Slicer
### add(PivotTable pivot, String destCellName, PivotField baseField) {#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, String destCellName, PivotField baseField)
```


Aggiungi un nuovo Slicer usando PivotTable come origine dati

**Example**

```
         slicers.add(pivot, "I3", pivot.getBaseFields().get(0));
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Oggetto PivotTable |
| destCellName | java.lang.String | La cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | The PivotField in PivotTable.BaseFields |

**Returns:**
int - Il nuovo indice di aggiunta Slicer
### add(PivotTable pivot, String destCellName, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-java.lang.String-int-}
```
public int add(PivotTable pivot, String destCellName, int baseFieldIndex)
```


Aggiungi un nuovo Slicer usando PivotTable come origine dati

**Example**

```
         slicers.add(pivot, "E20", 0);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Oggetto PivotTable |
| destCellName | java.lang.String | La cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| baseFieldIndex | int | L'indice del PivotField in PivotTable.BaseFields |

**Returns:**
int - Il nuovo indice di aggiunta Slicer
### add(PivotTable pivot, String destCellName, String baseFieldName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivot, String destCellName, String baseFieldName)
```


Aggiungi un nuovo Slicer usando PivotTable come origine dati

**Example**

```
         slicers.add(pivot, "E3", "fruit");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Oggetto PivotTable |
| destCellName | java.lang.String | La cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| baseFieldName | java.lang.String | Il nome del PivotField in PivotTable.BaseFields |

**Returns:**
int - Il nuovo indice di aggiunta Slicer
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


Cancella tutti i Slicer.

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
public Slicer get(int index)
```


Ottiene il Slicer per indice.

**Example**

```
         Slicer slicerByIndex = slicers.get(0);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
### get(String name) {#get-java.lang.String-}
```
public Slicer get(String name)
```


Ottiene il Slicer per nome del slicer.

**Example**

```
         Slicer slicerByName = slicers.get("fruit");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
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




### remove(Slicer slicer) {#remove-com.aspose.cells.Slicer-}
```
public void remove(Slicer slicer)
```


Rimuovi lo Slicer specificato

**Example**

```
         Slicer delSlicer = slicers.get(0);
         slicers.remove(delSlicer);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| slicer | [Slicer](../../com.aspose.cells/slicer) | L'oggetto Slicer |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina lo Slicer all'indice specificato

**Example**

```
         slicers.removeAt(1);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice di posizione nella collezione Slicer |

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

