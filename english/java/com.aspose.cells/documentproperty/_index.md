---
title: DocumentProperty
second_title: Aspose.Cells for Java API Reference
description: Represents a custom or built-in document property.
type: docs
weight: 177
url: /java/com.aspose.cells/documentproperty/
---

**Inheritance:**
java.lang.Object
```
public class DocumentProperty
```

Represents a custom or built-in document property.

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
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Returns the name of the property. |
| [getSource()](#getSource--) | The linked content source. |
| [getType()](#getType--) | Gets the data type of the property. |
| [getValue()](#getValue--) | the value of the property. |
| [hashCode()](#hashCode--) |  |
| [isGeneratedName()](#isGeneratedName--) | Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API. |
| [isLinkedToContent()](#isLinkedToContent--) | Indicates whether this property is linked to content |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setValue(Object value)](#setValue-java.lang.Object-) | For the description of this property, please see [getValue()](../../com.aspose.cells/documentproperty\#getValue--) |
| [toBool()](#toBool--) | Returns the property value as bool. |
| [toDateTime()](#toDateTime--) | Returns the property value as DateTime in local timezone. |
| [toDouble()](#toDouble--) | Returns the property value as double. |
| [toInt()](#toInt--) | Returns the property value as integer. |
| [toString()](#toString--) | Returns the property value as a string. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
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


Returns the name of the property.

**Returns:**
java.lang.String
### getSource() {#getSource--}
```
public String getSource()
```


The linked content source.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Gets the data type of the property.

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


the value of the property.

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


Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API.

**Returns:**
boolean
### isLinkedToContent() {#isLinkedToContent--}
```
public boolean isLinkedToContent()
```


Indicates whether this property is linked to content

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


For the description of this property, please see [getValue()](../../com.aspose.cells/documentproperty\#getValue--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |

### toBool() {#toBool--}
```
public boolean toBool()
```


Returns the property value as bool.

Throws an exception if the property type is not PropertyType.Boolean.

**Returns:**
boolean
### toDateTime() {#toDateTime--}
```
public DateTime toDateTime()
```


Returns the property value as DateTime in local timezone.

Throws an exception if the property type is not PropertyType.Date.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### toDouble() {#toDouble--}
```
public double toDouble()
```


Returns the property value as double. Throws an exception if the property type is not PropertyType.Float.

**Returns:**
double
### toInt() {#toInt--}
```
public int toInt()
```


Returns the property value as integer. Throws an exception if the property type is not PropertyType.Number.

**Returns:**
int
### toString() {#toString--}
```
public String toString()
```


Returns the property value as a string.

Converts a number property using Object.ToString(). Converts a boolean property into "Y" or "N". Converts a date property into a short date string.

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

