---
title: "ChartCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von Objekten."
type: docs
url: /de/java/com.aspose.cells/chartcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ChartCollection extends CollectionBase
```

Kapselt eine Sammlung von [Chart](../../com.aspose.cells/chart)-Objekten.

**Example**

```
         Workbook workbook = new Workbook();
 
         ChartCollection charts = workbook.getWorksheets().get(0).getCharts();
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-byte---java.lang.String-boolean-int-int-int-int-) | Fügt ein Diagramm mit vordefinierter Vorlage hinzu. |
| [add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn)](#add-int-int-int-int-int-) | Fügt ein Diagramm zur Sammlung hinzu. |
| [add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-boolean-int-int-int-int-) | Fügt ein Diagramm zur Sammlung hinzu. |
| [add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-int-int-int-int-) | Fügt ein Diagramm zur Sammlung hinzu. |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [addFloatingChart(int type, int left, int top, int width, int height)](#addFloatingChart-int-int-int-int-int-) | Fügt ein Diagramm zur Sammlung hinzu. |
| [clear()](#clear--) | Alle Diagramme löschen. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Liefert das [Chart](../../com.aspose.cells/chart)-Element am angegebenen Index. |
| [get(String name)](#get-java.lang.String-) | Liefert das Diagramm nach dem Namen. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Chart chart)](#remove-com.aspose.cells.Chart-) | Entfernt das spezifische Diagramm. |
| [removeAt(int index)](#removeAt-int-) | Entfernt ein Diagramm am spezifischen Index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-byte---java.lang.String-boolean-int-int-int-int-}
```
public int add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


Fügt ein Diagramm mit vordefinierter Vorlage hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Daten | byte[] | Die Daten der Diagrammvorlagendatei (.crtx). |
| dataRange | java.lang.String | Gibt den Datenbereich des Diagramms an |
| isVertical | boolean | Gibt an, ob die Serie aus einem Zellwertbereich zeilenweise oder spaltenweise geplottet werden soll. |
| topRow | int | Index der oberen linken Zeile. |
| leftColumn | int | Index der oberen linken Spalte. |
| rightRow | int | Index der unteren rechten Zeile |
| bottomColumn | int | Index der unteren rechten Spalte |

**Returns:**
int - [Chart](../../com.aspose.cells/chart)-Objektindex.
### add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn) {#add-int-int-int-int-int-}
```
public int add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Fügt ein Diagramm zur Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Diagrammtyp |
| topRow | int | Index der oberen linken Zeile. |
| leftColumn | int | Index der oberen linken Spalte. |
| bottomRow | int | Index der unteren rechten Zeile |
| rightColumn | int | Index der unteren rechten Spalte |

**Returns:**
int - [Chart](../../com.aspose.cells/chart)-Objektindex.
### add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-boolean-int-int-int-int-}
```
public int add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


Fügt ein Diagramm zur Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Diagrammtyp |
| dataRange | java.lang.String | Gibt den Datenbereich des Diagramms an |
| isVertical | boolean | Gibt an, ob die Serie aus einem Zellwertbereich zeilenweise oder spaltenweise geplottet werden soll. |
| topRow | int | Index der oberen linken Zeile. |
| leftColumn | int | Index der oberen linken Spalte. |
| rightRow | int | Index der unteren rechten Zeile |
| bottomColumn | int | Index der unteren rechten Spalte |

**Returns:**
int - [Chart](../../com.aspose.cells/chart)-Objektindex.
### add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-int-int-int-int-}
```
public int add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


Fügt ein Diagramm zur Sammlung hinzu.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [add(int,String,boolean,int,int,int,int)](../../com.aspose.cells/chartcollection\\#add-int-String-boolean-int-int-int-int-) Eigenschaft. Diese Eigenschaft wird 12 Monate nach Mai 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Diagrammtyp |
| dataRange | java.lang.String | Gibt den Datenbereich des Diagramms an |
| topRow | int | Index der oberen linken Zeile. |
| leftColumn | int | Index der oberen linken Spalte. |
| rightRow | int | Index der unteren rechten Zeile |
| bottomColumn | int | Index der unteren rechten Spalte |

**Returns:**
int - [Chart](../../com.aspose.cells/chart)-Objektindex.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Fügt ein Element zur CollectionBase-Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Das Objekt, das zur CollectionBase-Instanz hinzugefügt werden soll. |

**Returns:**
int - Die Position, an der das neue Element eingefügt wurde.
### addFloatingChart(int type, int left, int top, int width, int height) {#addFloatingChart-int-int-int-int-int-}
```
public int addFloatingChart(int type, int left, int top, int width, int height)
```


Fügt ein Diagramm zur Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Diagrammtyp |
| links | int | Der x‑Versatz zur Ecke |
| oben | int | Der y‑Versatz zur Ecke |
| Breite | int | Die Diagrammbreite |
| Höhe | int | Die Diagrammhöhe |

**Returns:**
int - [Chart](../../com.aspose.cells/chart)-Objektindex.
### clear() {#clear--}
```
public void clear()
```


Alle Diagramme löschen.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Gibt zurück, ob die Instanz dieses Objekt enthält

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Testobjekt |

**Returns:**
boolean - Ob die Instanz dieses Objekt enthält
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
public Chart get(int index)
```


Liefert das [Chart](../../com.aspose.cells/chart)-Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

**Returns:**
[Chart](../../com.aspose.cells/chart) - The element at the specified index.
### get(String name) {#get-java.lang.String-}
```
public Chart get(String name)
```


Liefert das Diagramm nach dem Namen.

**Remarks**

Der Standarddiagrammname ist null. Daher müssen Sie den Namen des Diagramms explizit festlegen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Diagrammname. |

**Returns:**
[Chart](../../com.aspose.cells/chart) - The chart.
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


Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.

**Returns:**
int - Die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.
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


Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |

**Returns:**
int - Der Index des Wertes, falls in der Liste gefunden; sonst -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft.

**Returns:**
java.util.Iterator - Ein Iterator für die CollectionBase-Instanz.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(Chart chart) {#remove-com.aspose.cells.Chart-}
```
public void remove(Chart chart)
```


Entfernt das spezifische Diagramm.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| chart | [Chart](../../com.aspose.cells/chart) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entfernt ein Diagramm am spezifischen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Diagrammindex. |

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

