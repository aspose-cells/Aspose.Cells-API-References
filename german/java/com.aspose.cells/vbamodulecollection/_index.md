---
title: "VbaModuleCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Liste von dar"
type: docs
url: /de/java/com.aspose.cells/vbamodulecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VbaModuleCollection extends CollectionBase
```

Stellt die Liste von [VbaModule](../../com.aspose.cells/vbamodule) dar.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject(); 
         // Add a new module.
         vbaProject.getModules().add(VbaModuleType.CLASS, "test");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(Worksheet sheet)](#add-com.aspose.cells.Worksheet-) | Fügt ein Modul für ein Arbeitsblatt hinzu. |
| [add(int type, String name)](#add-int-java.lang.String-) | Fügt ein Modul hinzu. |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [addDesignerStorage(String name, byte[] data)](#addDesignerStorage-java.lang.String-byte---) |  |
| [addUserForm(String name, String codes, byte[] designerStorage)](#addUserForm-java.lang.String-java.lang.String-byte---) | Fügt ein Benutzerformular in das VBA-Projekt ein. |
| [clear()](#clear--) | Entfernt alle Objekte aus der CollectionBase-Instanz. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ruft [VbaModule](../../com.aspose.cells/vbamodule) in der Liste nach dem Index ab. |
| [get(String name)](#get-java.lang.String-) | Ruft [VbaModule](../../com.aspose.cells/vbamodule) in der Liste nach dem Namen ab. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [getDesignerStorage(String name)](#getDesignerStorage-java.lang.String-) | Stellt die Daten des Designers dar. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Worksheet sheet)](#remove-com.aspose.cells.Worksheet-) | Entfernt das Modul für ein Arbeitsblatt. |
| [remove(String name)](#remove-java.lang.String-) | Entferne das Modul nach dem Namen. |
| [removeAt(int index)](#removeAt-int-) | Entfernt das Element am angegebenen Index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Worksheet sheet) {#add-com.aspose.cells.Worksheet-}
```
public int add(Worksheet sheet)
```


Fügt ein Modul für ein Arbeitsblatt hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | Das Arbeitsblatt |

**Returns:**
int -
### add(int type, String name) {#add-int-java.lang.String-}
```
public int add(int type, String name)
```


Fügt ein Modul hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [VbaModuleType](../../com.aspose.cells/vbamoduletype). Der Typ des Moduls. |
| Name | java.lang.String | Der Name des Moduls. |

**Returns:**
int -
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
### addDesignerStorage(String name, byte[] data) {#addDesignerStorage-java.lang.String-byte---}
```
public void addDesignerStorage(String name, byte[] data)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |
| Daten | byte[] |  |

### addUserForm(String name, String codes, byte[] designerStorage) {#addUserForm-java.lang.String-java.lang.String-byte---}
```
public int addUserForm(String name, String codes, byte[] designerStorage)
```


Fügt ein Benutzerformular in das VBA-Projekt ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des Benutzerformulars |
| Codes | java.lang.String | Die Codes für das Benutzerformular |
| designerStorage | byte[] | die Designer-Einstellung zum Benutzerformular |

**Returns:**
int -
### clear() {#clear--}
```
public void clear()
```


Entfernt alle Objekte aus der CollectionBase-Instanz.

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
public VbaModule get(int index)
```


Ruft [VbaModule](../../com.aspose.cells/vbamodule) in der Liste nach dem Index ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index. |

**Returns:**
[VbaModule](../../com.aspose.cells/vbamodule) - 
### get(String name) {#get-java.lang.String-}
```
public VbaModule get(String name)
```


Ruft [VbaModule](../../com.aspose.cells/vbamodule) in der Liste nach dem Namen ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des Moduls. |

**Returns:**
[VbaModule](../../com.aspose.cells/vbamodule) - 
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
### getDesignerStorage(String name) {#getDesignerStorage-java.lang.String-}
```
public byte[] getDesignerStorage(String name)
```


Stellt die Daten des Designers dar.

**Remarks**

Wir unterstützen das Parsen nicht. Nur zum Kopieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
byte[]
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




### remove(Worksheet sheet) {#remove-com.aspose.cells.Worksheet-}
```
public void remove(Worksheet sheet)
```


Entfernt das Modul für ein Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | Das Arbeitsblatt |

### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


Entferne das Modul nach dem Namen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entfernt das Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des zu entfernenden Elements. |

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

