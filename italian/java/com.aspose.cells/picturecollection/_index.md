---
title: "PictureCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula una raccolta di oggetti."
type: docs
url: /it/java/com.aspose.cells/picturecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PictureCollection extends CollectionBase
```

Incapsula una raccolta di oggetti [Picture](../../com.aspose.cells/picture).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //get PictureCollection
         PictureCollection pictures = workbook.getWorksheets().get(0).getPictures();
 
         //do your business
 
         //Save the excel file.
         workbook.save("result.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#add-int-int-int-int-java.io.InputStream-) | Aggiunge un'immagine alla collezione. |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)](#add-int-int-int-int-java.lang.String-) | Aggiunge un'immagine alla collezione. |
| [add(int topRow, int leftColumn, InputStream stream)](#add-int-int-java.io.InputStream-) | Aggiunge un'immagine alla collezione. |
| [add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#add-int-int-java.io.InputStream-int-int-) | Aggiunge un'immagine alla collezione. |
| [add(int topRow, int leftColumn, String fileName)](#add-int-int-java.lang.String-) | Aggiunge un'immagine alla collezione. |
| [add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)](#add-int-int-java.lang.String-int-int-) | Aggiunge un'immagine alla collezione. |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [camera(int row, int column, String range)](#camera-int-int-java.lang.String-) | Scatta una foto dell'intervallo. |
| [clear()](#clear--) | Cancella tutte le immagini. |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene l'elemento [Picture](../../com.aspose.cells/picture) all'indice specificato. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Rimuove le forme all'indice specifico |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#add-int-int-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


Aggiunge un'immagine alla collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| bottomRow | int | Indice della riga in basso a destra |
| rightColumn | int | Indice della colonna in basso a destra |
| stream | java.io.InputStream | Oggetto stream che contiene i dati dell'immagine. |

**Returns:**
int - indice dell'oggetto [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName) {#add-int-int-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)
```


Aggiunge un'immagine alla collezione.

**Example**

```
         //add a picture
         pictures.add(1, 1, 5, 5, "image.jpg");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| bottomRow | int | Indice della riga in basso a destra |
| rightColumn | int | Indice della colonna in basso a destra |
| fileName | java.lang.String | Nome file dell'immagine. |

**Returns:**
int - indice dell'oggetto [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, InputStream stream) {#add-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, InputStream stream)
```


Aggiunge un'immagine alla collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| stream | java.io.InputStream | Oggetto stream che contiene i dati dell'immagine. |

**Returns:**
int - indice dell'oggetto [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#add-int-int-java.io.InputStream-int-int-}
```
public int add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


Aggiunge un'immagine alla collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| stream | java.io.InputStream | Oggetto stream che contiene i dati dell'immagine. |
| widthScale | int | Scala della larghezza dell'immagine, in percentuale. |
| heightScale | int | Scala dell'altezza dell'immagine, in percentuale. |

**Returns:**
int - indice dell'oggetto [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, String fileName) {#add-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, String fileName)
```


Aggiunge un'immagine alla collezione.

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| fileName | java.lang.String | Nome file dell'immagine. |

**Returns:**
int - indice dell'oggetto [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale) {#add-int-int-java.lang.String-int-int-}
```
public int add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)
```


Aggiunge un'immagine alla collezione.

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg", 50, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| fileName | java.lang.String | Nome file dell'immagine. |
| widthScale | int | Scala della larghezza dell'immagine, in percentuale. |
| heightScale | int | Scala dell'altezza dell'immagine, in percentuale. |

**Returns:**
int - indice dell'oggetto [Picture](../../com.aspose.cells/picture).
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
### camera(int row, int column, String range) {#camera-int-int-java.lang.String-}
```
public int camera(int row, int column, String range)
```


Scatta una foto dell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice di riga di questa immagine. |
| colonna | int | L'indice di colonna di questa immagine. |
| intervallo | java.lang.String | L'area che richiede la fotografia |

**Returns:**
int -
### clear() {#clear--}
```
public void clear()
```


Cancella tutte le immagini.

**Example**

```
         //clear
         pictures.clear();
```

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
public Picture get(int index)
```


Ottiene l'elemento [Picture](../../com.aspose.cells/picture) all'indice specificato.

**Example**

```
         //get picture collection
         //PictureCollection pictures = workbook.Worksheets[0].Pictures;
         //add a picture
         int index = pictures.add(1, 1, "image.png");
         //get the picture
         Picture pic = pictures.get(index);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - The element at the specified index.
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


Rimuove le forme all'indice specifico

**Example**

```
         //add a picture
         int index2 = pictures.add(1, 1, "image.png");
         //delete
         pictures.removeAt(index2);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

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

