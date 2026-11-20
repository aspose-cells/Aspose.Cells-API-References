---
title: "GridWorksheetCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula una raccolta di oggetti."
type: docs
url: /it/java/com.aspose.gridweb/gridworksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class GridWorksheetCollection extends CollectionBase
```

Incapsula una raccolta di oggetti [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add()](#add--) | Aggiunge un foglio di lavoro alla raccolta. |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [add(String sheetName)](#add-java.lang.String-) | Aggiunge un foglio di lavoro alla raccolta. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Aggiunge un foglio di lavoro alla raccolta e copia i dati da un foglio di lavoro esistente. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Aggiunge un foglio di lavoro alla raccolta e copia i dati da un foglio di lavoro esistente. |
| [calculateFormula()](#calculateFormula--) | Calcola il risultato delle formule. |
| [clear()](#clear--) | Cancella tutti i fogli di lavoro. |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene l'elemento [GridWorksheet](../../com.aspose.gridweb/gridworksheet) all'indice specificato. |
| [get(String sheetName)](#get-java.lang.String-) | Ottiene l'elemento [GridWorksheet](../../com.aspose.gridweb/gridworksheet) con il nome specificato. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Rappresenta l'indice del foglio di lavoro attivo quando il foglio di calcolo è aperto. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Restituisce la dimensione dell'enumeratore |
| [getDefaultFontName()](#getDefaultFontName--) | Ottiene il nome del carattere predefinito del controllo. |
| [getDefaultFontSize()](#getDefaultFontSize--) | ????????? |
| [getNames()](#getNames--) | Ottiene la raccolta di tutti gli oggetti Name nel foglio di calcolo. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Ottiene il separatore decimale per la formattazione/analisi dei valori numerici. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [insert(int index, String sheetName)](#insert-int-java.lang.String-) | Inserisci un foglio di lavoro. |
| [iterator()](#iterator--) | Restituisce l'enumeratore delle righe |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Rimuove l'elemento a un indice specificato. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Rimuove l'elemento a un nome specificato. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Rappresenta l'indice del foglio di lavoro attivo quando il foglio di calcolo è aperto. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Imposta il nome del carattere predefinito del controllo. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | ????????? |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Imposta il separatore decimale per la formattazione/analisi dei valori numerici. |
| [setVisible(String sheetName, boolean isVisible)](#setVisible-java.lang.String-boolean-) | Imposta la visibilità per il foglio. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | Scambia i due fogli. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Aggiunge un foglio di lavoro alla raccolta.

**Returns:**
int - indice dell'oggetto [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
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
### add(String sheetName) {#add-java.lang.String-}
```
public GridWorksheet add(String sheetName)
```


Aggiunge un foglio di lavoro alla raccolta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | java.lang.String | Nome del foglio di lavoro |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) object.
### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


Aggiunge un foglio di lavoro alla raccolta e copia i dati da un foglio di lavoro esistente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | int | Indice del foglio di lavoro di origine. |

**Returns:**
int - indice dell'oggetto [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


Aggiunge un foglio di lavoro alla raccolta e copia i dati da un foglio di lavoro esistente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | java.lang.String | Nome del foglio di lavoro di origine. |

**Returns:**
int - indice dell'oggetto [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Calcola il risultato delle formule.

### clear() {#clear--}
```
public void clear()
```


Cancella tutti i fogli di lavoro.

**Remarks**

Una cartella di lavoro deve contenere un foglio di lavoro.

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
public GridWorksheet get(int index)
```


Ottiene l'elemento [GridWorksheet](../../com.aspose.gridweb/gridworksheet) all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public GridWorksheet get(String sheetName)
```


Ottiene l'elemento [GridWorksheet](../../com.aspose.gridweb/gridworksheet) con il nome specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | java.lang.String | Il nome del foglio di lavoro. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The GridWorksheet with the name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Rappresenta l'indice del foglio di lavoro attivo quando il foglio di calcolo è aperto.

**Remarks**

L'indice del foglio è basato su zero.

**Returns:**
int
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


Restituisce la dimensione dell'enumeratore

**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Ottiene il nome del carattere predefinito del controllo.

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```


?????????

**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getNames() {#getNames--}
```
public GridNameCollection getNames()
```


Ottiene la raccolta di tutti gli oggetti Name nel foglio di calcolo.

**Returns:**
[GridNameCollection](../../com.aspose.gridweb/gridnamecollection)
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


Ottiene il separatore decimale per la formattazione/analisi dei valori numerici. Il valore predefinito è il separatore decimale della Regione corrente.

**Returns:**
char
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
### insert(int index, String sheetName) {#insert-int-java.lang.String-}
```
public GridWorksheet insert(int index, String sheetName)
```


Inserisci un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice del foglio |
| sheetName | java.lang.String |  |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### iterator() {#iterator--}
```
public Iterator iterator()
```


Restituisce l'enumeratore delle righe

**Returns:**
java.util.Iterator - L'enumeratore delle righe
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


Rimuove l'elemento a un indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | Il valore indice dell'elemento da rimuovere. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


Rimuove l'elemento a un nome specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome dell'elemento da rimuovere. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Rappresenta l'indice del foglio di lavoro attivo quando il foglio di calcolo è aperto.

**Remarks**

L'indice del foglio è basato su zero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Imposta il nome del carattere predefinito del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


?????????

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


Imposta il separatore decimale per la formattazione/analisi dei valori numerici. Il valore predefinito è il separatore decimale della regione corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char |  |

### setVisible(String sheetName, boolean isVisible) {#setVisible-java.lang.String-boolean-}
```
public void setVisible(String sheetName, boolean isVisible)
```


Imposta la visibilità per il foglio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | java.lang.String | Nome del foglio di lavoro di origine. |
| isVisible | boolean | Se il foglio di lavoro è visibile |

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


Scambia i due fogli.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex1 | int | Il primo foglio di lavoro. |
| sheetIndex2 | int | Il secondo foglio di lavoro. |

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

