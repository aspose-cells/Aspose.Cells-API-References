---
title: "CustomDocumentPropertyCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Eine Sammlung benutzerdefinierter Dokumenteigenschaften."
type: docs
url: /de/java/com.aspose.cells/customdocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class CustomDocumentPropertyCollection extends DocumentPropertyCollection
```

Eine Sammlung benutzerdefinierter Dokumenteigenschaften.

**Remarks**

Jedes Objekt stellt eine benutzerdefinierte Eigenschaft eines Containerdokuments dar.

**Example**

```
         //Instantiate a Workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Retrieve a list of all custom document properties of the Excel file
         CustomDocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.Boolean**. |
| [add(String name, DateTime value)](#add-java.lang.String-com.aspose.cells.DateTime-) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.DateTime**. |
| [add(String name, double value)](#add-java.lang.String-double-) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.Float**. |
| [add(String name, int value)](#add-java.lang.String-int-) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.Number**. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.String**. |
| [addLinkToContent(String name, String source)](#addLinkToContent-java.lang.String-java.lang.String-) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft, die mit Inhalt verknüpft ist. |
| [clear()](#clear--) | Entfernt alle Objekte aus der CollectionBase-Instanz. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [contains(String name)](#contains-java.lang.String-) | Gibt true zurück, wenn eine Eigenschaft mit dem angegebenen Namen in der Sammlung existiert. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gibt ein [DocumentProperty](../../com.aspose.cells/documentproperty)-Objekt nach Index zurück. |
| [get(String name)](#get-java.lang.String-) | Gibt ein [DocumentProperty](../../com.aspose.cells/documentproperty)-Objekt nach dem Namen der Eigenschaft zurück. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [indexOf(String name)](#indexOf-java.lang.String-) | Ermittelt den Index einer Eigenschaft nach Namen. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | Entfernt eine Eigenschaft mit dem angegebenen Namen aus der Sammlung. |
| [removeAt(int index)](#removeAt-int-) | Entfernt eine Eigenschaft am angegebenen Index. |
| [toString()](#toString--) |  |
| [updateLinkedPropertyValue()](#updateLinkedPropertyValue--) | Aktualisiert die Werte aller benutzerdefinierten Eigenschaften, die mit Inhalt verknüpft sind (verwende den Zellenwert des verknüpften Bereichs, um den Wert der benutzerdefinierten Eigenschaft zu aktualisieren). |
| [updateLinkedRange()](#updateLinkedRange--) | Aktualisiert alle Bereiche, die mit benutzerdefinierten Eigenschaften verknüpft sind (verwendet den Wert der benutzerdefinierten Dokumenteigenschaft, um den Zellenwert des verknüpften Bereichs zu aktualisieren). |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public DocumentProperty add(String name, boolean value)
```


Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.Boolean**.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name der Eigenschaft. |
| Wert | boolean | Der Wert der Eigenschaft. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, DateTime value) {#add-java.lang.String-com.aspose.cells.DateTime-}
```
public DocumentProperty add(String name, DateTime value)
```


Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.DateTime**.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name der Eigenschaft. |
| value | [DateTime](../../com.aspose.cells/datetime) | Der Wert der Eigenschaft. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public DocumentProperty add(String name, double value)
```


Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.Float**.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name der Eigenschaft. |
| Wert | double | Der Wert der Eigenschaft. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, int value) {#add-java.lang.String-int-}
```
public DocumentProperty add(String name, int value)
```


Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.Number**.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name der Eigenschaft. |
| Wert | int | Der Wert der Eigenschaft. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public DocumentProperty add(String name, String value)
```


Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.String**.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name der Eigenschaft. |
| Wert | java.lang.String | Der Wert der Eigenschaft. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### addLinkToContent(String name, String source) {#addLinkToContent-java.lang.String-java.lang.String-}
```
public DocumentProperty addLinkToContent(String name, String source)
```


Erstellt eine neue benutzerdefinierte Dokumenteigenschaft, die mit Inhalt verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name der Eigenschaft. |
| Quelle | java.lang.String | Die Quelle der Eigenschaft. Sie sollte der Name des benannten Bereichs sein. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
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
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


Gibt true zurück, wenn eine Eigenschaft mit dem angegebenen Namen in der Sammlung existiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Groß-/Kleinschreibung ignorierende Name der Eigenschaft. |

**Returns:**
boolean - True, wenn die Eigenschaft in der Sammlung existiert; sonst false.
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
public DocumentProperty get(int index)
```


Gibt ein [DocumentProperty](../../com.aspose.cells/documentproperty)-Objekt nach Index zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| index | int | Nullbasierter Index des zu holenden [DocumentProperty](../../com.aspose.cells/documentproperty). |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


Gibt ein [DocumentProperty](../../com.aspose.cells/documentproperty)-Objekt nach dem Namen der Eigenschaft zurück.

**Remarks**

Gibt null zurück, wenn eine Eigenschaft mit dem angegebenen Namen nicht gefunden wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Groß-/Kleinschreibung ignorierende Name der abzurufenden Eigenschaft. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
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
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


Ermittelt den Index einer Eigenschaft nach Namen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Groß-/Kleinschreibung ignorierende Name der Eigenschaft. |

**Returns:**
int - Der nullbasierte Index. Negativer Wert, wenn nicht gefunden.
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




### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


Entfernt eine Eigenschaft mit dem angegebenen Namen aus der Sammlung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Groß-/Kleinschreibung ignorierende Name der Eigenschaft. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entfernt eine Eigenschaft am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateLinkedPropertyValue() {#updateLinkedPropertyValue--}
```
public void updateLinkedPropertyValue()
```


Aktualisiert die Werte aller benutzerdefinierten Eigenschaften, die mit Inhalt verknüpft sind (verwende den Zellenwert des verknüpften Bereichs, um den Wert der benutzerdefinierten Eigenschaft zu aktualisieren).

### updateLinkedRange() {#updateLinkedRange--}
```
public void updateLinkedRange()
```


Aktualisiert alle Bereiche, die mit benutzerdefinierten Eigenschaften verknüpft sind (verwendet den Wert der benutzerdefinierten Dokumenteigenschaft, um den Zellenwert des verknüpften Bereichs zu aktualisieren).

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

