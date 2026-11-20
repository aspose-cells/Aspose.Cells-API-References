---
title: "DocumentProperty"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine benutzerdefinierte oder integrierte Dokumenteigenschaft dar."
type: docs
url: /de/java/com.aspose.cells/documentproperty/
---

**Inheritance:**
java.lang.Object
```
public class DocumentProperty
```

Stellt eine benutzerdefinierte oder integrierte Dokumenteigenschaft dar.

**Example**

```
         //Instantiate a Workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Retrieve a list of all custom document properties of the Excel file
         DocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
 
         //Accessng a custom document property by using the property index
         DocumentProperty customProperty1 = customProperties.get(3);
 
         //Accessng a custom document property by using the property name
         DocumentProperty customProperty2 = customProperties.get("Owner");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Gibt den Namen der Eigenschaft zurück. |
| [getSource()](#getSource--) | Die verknüpfte Inhaltsquelle. |
| [getType()](#getType--) | Ruft den Datentyp der Eigenschaft ab. |
| [getValue()](#getValue--) | Liefert den Wert der Eigenschaft. |
| [hashCode()](#hashCode--) |  |
| [isGeneratedName()](#isGeneratedName--) | Gibt true zurück, wenn diese Eigenschaft keinen Namen im OLE2-Speicher hat und ein eindeutiger Name nur für die öffentliche API generiert wurde. |
| [isLinkedToContent()](#isLinkedToContent--) | Gibt an, ob diese Eigenschaft mit Inhalt verknüpft ist |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setValue(Object value)](#setValue-java.lang.Object-) | Setzt den Wert der Eigenschaft. |
| [toBool()](#toBool--) | Gibt den Eigenschaftswert als bool zurück. |
| [toDateTime()](#toDateTime--) | Gibt den Eigenschaftswert als DateTime in der lokalen Zeitzone zurück. |
| [toDouble()](#toDouble--) | Gibt den Eigenschaftswert als double zurück. |
| [toInt()](#toInt--) | Gibt den Eigenschaftswert als integer zurück. |
| [toString()](#toString--) | Gibt den Eigenschaftswert als Zeichenkette zurück. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


Gibt den Namen der Eigenschaft zurück.

**Returns:**
java.lang.String
### getSource() {#getSource--}
```
public String getSource()
```


Die verknüpfte Inhaltsquelle.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Ruft den Datentyp der Eigenschaft ab.

Siehe [PropertyType](../../com.aspose.cells/propertytype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Liefert den Wert der Eigenschaft.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGeneratedName() {#isGeneratedName--}
```
public boolean isGeneratedName()
```


Gibt true zurück, wenn diese Eigenschaft keinen Namen im OLE2-Speicher hat und ein eindeutiger Name nur für die öffentliche API generiert wurde.

**Returns:**
boolean
### isLinkedToContent() {#isLinkedToContent--}
```
public boolean isLinkedToContent()
```


Gibt an, ob diese Eigenschaft mit Inhalt verknüpft ist

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Setzt den Wert der Eigenschaft.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object |  |

### toBool() {#toBool--}
```
public boolean toBool()
```


Gibt den Eigenschaftswert als bool zurück.

**Remarks**

Wirft eine Ausnahme, wenn der Eigenschaftstyp nicht PropertyType.Boolean ist.

**Returns:**
boolean
### toDateTime() {#toDateTime--}
```
public DateTime toDateTime()
```


Gibt den Eigenschaftswert als DateTime in der lokalen Zeitzone zurück.

**Remarks**

Wirft eine Ausnahme, wenn der Eigenschaftstyp nicht PropertyType.Date ist.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### toDouble() {#toDouble--}
```
public double toDouble()
```


Gibt den Eigenschaftswert als double zurück.

**Remarks**

Wirft eine Ausnahme, wenn der Eigenschaftstyp nicht PropertyType.Float ist.

**Returns:**
double
### toInt() {#toInt--}
```
public int toInt()
```


Gibt den Eigenschaftswert als integer zurück.

**Remarks**

Wirft eine Ausnahme, wenn der Eigenschaftstyp nicht PropertyType.Number ist.

**Returns:**
int
### toString() {#toString--}
```
public String toString()
```


Gibt den Eigenschaftswert als Zeichenkette zurück.

**Remarks**

Konvertiert eine Zahleneigenschaft mit Object.ToString(). Konvertiert eine boolesche Eigenschaft in "Y" oder "N". Konvertiert eine Datumseigenschaft in eine kurze Datumszeichenkette.

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

