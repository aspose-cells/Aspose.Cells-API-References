---
title: "DocumentProperty"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en anpassad eller inbyggd dokumentegenskap."
type: docs
url: /sv/java/com.aspose.cells/documentproperty/
---

**Inheritance:**
java.lang.Object
```
public class DocumentProperty
```

Representerar en anpassad eller inbyggd dokumentegenskap.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Returnerar namnet på egenskapen. |
| [getSource()](#getSource--) | Den länkade innehållskällan. |
| [getType()](#getType--) | Hämtar datatypen för egenskapen. |
| [getValue()](#getValue--) | Hämtar värdet på egenskapen. |
| [hashCode()](#hashCode--) |  |
| [isGeneratedName()](#isGeneratedName--) | Returnerar true om denna egenskap inte har ett namn i OLE2-lagringen och ett unikt namn genererades endast för det offentliga API:et. |
| [isLinkedToContent()](#isLinkedToContent--) | Indikerar om denna egenskap är länkad till innehåll |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setValue(Object value)](#setValue-java.lang.Object-) | Ställer in värdet på egenskapen. |
| [toBool()](#toBool--) | Returnerar egenskapsvärdet som bool. |
| [toDateTime()](#toDateTime--) | Returnerar egenskapsvärdet som DateTime i lokal tidszon. |
| [toDouble()](#toDouble--) | Returnerar egenskapsvärdet som double. |
| [toInt()](#toInt--) | Returnerar egenskapsvärdet som integer. |
| [toString()](#toString--) | Returnerar egenskapsvärdet som en sträng. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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


Returnerar namnet på egenskapen.

**Returns:**
java.lang.String
### getSource() {#getSource--}
```
public String getSource()
```


Den länkade innehållskällan.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Hämtar datatypen för egenskapen.

Se [PropertyType](../../com.aspose.cells/propertytype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Hämtar värdet på egenskapen.

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


Returnerar true om denna egenskap inte har ett namn i OLE2-lagringen och ett unikt namn genererades endast för det offentliga API:et.

**Returns:**
boolean
### isLinkedToContent() {#isLinkedToContent--}
```
public boolean isLinkedToContent()
```


Indikerar om denna egenskap är länkad till innehåll

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


Ställer in värdet på egenskapen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

### toBool() {#toBool--}
```
public boolean toBool()
```


Returnerar egenskapsvärdet som bool.

**Remarks**

Kastar ett undantag om egenskapstypen inte är PropertyType.Boolean.

**Returns:**
boolean
### toDateTime() {#toDateTime--}
```
public DateTime toDateTime()
```


Returnerar egenskapsvärdet som DateTime i lokal tidszon.

**Remarks**

Kastar ett undantag om egenskapstypen inte är PropertyType.Date.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### toDouble() {#toDouble--}
```
public double toDouble()
```


Returnerar egenskapsvärdet som double.

**Remarks**

Kastar ett undantag om egenskapstypen inte är PropertyType.Float.

**Returns:**
double
### toInt() {#toInt--}
```
public int toInt()
```


Returnerar egenskapsvärdet som integer.

**Remarks**

Kastar ett undantag om egenskapstypen inte är PropertyType.Number.

**Returns:**
int
### toString() {#toString--}
```
public String toString()
```


Returnerar egenskapsvärdet som en sträng.

**Remarks**

Konverterar en numerisk egenskap med hjälp av Object.ToString(). Konverterar en boolesk egenskap till "Y" eller "N". Konverterar en datumegenskap till en kort datumsträng.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

