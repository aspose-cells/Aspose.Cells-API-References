---
title: "ExternalLinkCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Sammlung externer Links in einer Arbeitsmappe dar."
type: docs
url: /de/java/com.aspose.cells/externallinkcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class ExternalLinkCollection implements Iterable
```

Stellt die Sammlung externer Links in einer Arbeitsmappe dar.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Change external link data source
         workbook.getWorksheets().getExternalLinks().get(0).setDataSource("d:\\link.xls");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(int directoryType, String fileName, String[] sheetNames)](#add-int-java.lang.String-java.lang.String---) | Füge einen externen Link hinzu. |
| [add(String fileName, String[] sheetNames)](#add-java.lang.String-java.lang.String---) | Fügt einen externen Link hinzu. |
| [clear()](#clear--) | Entfernt alle externen Links. |
| [clear(boolean updateReferencesAsLocal)](#clear-boolean-) | Entfernt alle externen Links. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Liefert das [ExternalLink](../../com.aspose.cells/externallink)-Element am angegebenen Index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Liefert die tatsächlich in der Sammlung enthaltene Anzahl von Elementen. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der diese Sammlung durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Entfernt den angegebenen externen Link aus der Arbeitsmappe. |
| [removeAt(int index, boolean updateReferencesAsLocal)](#removeAt-int-boolean-) | Entfernt den angegebenen externen Link aus der Arbeitsmappe. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int directoryType, String fileName, String[] sheetNames) {#add-int-java.lang.String-java.lang.String---}
```
public int add(int directoryType, String fileName, String[] sheetNames)
```


Füge einen externen Link hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| directoryType | int | [DirectoryType](../../com.aspose.cells/directorytype). Der Verzeichnistyp des Dateinamens. |
| fileName | java.lang.String | der Dateiname. |
| sheetNames | java.lang.String[] | Alle Blattnamen der externen Datei. |

**Returns:**
int - Die Position des externen Namens in dieser Liste.
### add(String fileName, String[] sheetNames) {#add-java.lang.String-java.lang.String---}
```
public int add(String fileName, String[] sheetNames)
```


Fügt einen externen Link hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der externe Dateiname. |
| sheetNames | java.lang.String[] | Alle Blattnamen der externen Datei. |

**Returns:**
int - Die Position des externen Namens in dieser Liste.
### clear() {#clear--}
```
public void clear()
```


Entfernt alle externen Links.

**Remarks**

Beim Entfernen externer Links werden alle Formeln, die auf sie verweisen, ebenfalls entfernt, da die Verweise ungültig werden.

### clear(boolean updateReferencesAsLocal) {#clear-boolean-}
```
public void clear(boolean updateReferencesAsLocal)
```


Entfernt alle externen Links.

**Remarks**

Wenn Referenzen aktualisiert werden müssen, werden diese Referenzen von externen Links in Formeln, sofern möglich, auf die aktuelle Arbeitsmappe geändert. Zum Beispiel lautet die ursprüngliche Formel einer Zelle "='externalsource.xlam'!customfunction()", nach dem Entfernen externer Links wird die Formel zu "=customfunction()"; Wenn die ursprüngliche Formel "='[externalsource.xlam]Sheet1'!$A$1" ist, hängt es davon ab, ob es ein Blatt mit dem Namen "Sheet1" in der aktuellen Arbeitsmappe gibt: ist dies der Fall, wird die Formel zu "=Sheet1!$A$1"; ist dies nicht der Fall, wird die Formel zu "=\#REF!$A$1".

Wenn Referenzen nicht aktualisiert werden müssen, werden alle Formeln mit Verweisen auf externe Links ebenfalls entfernt, da diese Verweise ungültig werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| updateReferencesAsLocal | boolean | Gibt an, ob alle Referenzen externer Links in Formeln auf Referenzen der aktuellen Arbeitsmappe selbst aktualisiert werden sollen. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public ExternalLink get(int index)
```


Liefert das [ExternalLink](../../com.aspose.cells/externallink)-Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

**Returns:**
[ExternalLink](../../com.aspose.cells/externallink) - The element at the specified index.
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


Liefert die tatsächlich in der Sammlung enthaltene Anzahl von Elementen.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Gibt einen Enumerator zurück, der diese Sammlung durchläuft.

**Returns:**
java.util.Iterator -
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


Entfernt den angegebenen externen Link aus der Arbeitsmappe.

**Remarks**

Beim Entfernen des externen Links werden alle Formeln, die darauf verweisen, ebenfalls entfernt, da die Referenzen ungültig werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index des zu entfernenden externen Links. |

### removeAt(int index, boolean updateReferencesAsLocal) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean updateReferencesAsLocal)
```


Entfernt den angegebenen externen Link aus der Arbeitsmappe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index des zu entfernenden externen Links. |
| updateReferencesAsLocal | boolean | Gibt an, ob alle Referenzen des angegebenen externen Links auf die Referenz der aktuellen Arbeitsmappe selbst aktualisiert werden sollen. Siehe [clear(boolean)](../../com.aspose.cells/externallinkcollection\#clear-boolean-) für weitere Details zu diesem Parameter. |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

