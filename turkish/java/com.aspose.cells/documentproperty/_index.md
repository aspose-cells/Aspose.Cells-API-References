---
title: "DocumentProperty"
second_title: "Aspose.Cells for Java API Referansı"
description: "Özel veya yerleşik bir belge özelliğini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/documentproperty/
---

**Inheritance:**
java.lang.Object
```
public class DocumentProperty
```

Özel veya yerleşik bir belge özelliğini temsil eder.

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
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Özelliğin adını döndürür. |
| [getSource()](#getSource--) | Bağlantılı içerik kaynağı. |
| [getType()](#getType--) | Özelliğin veri tipini alır. |
| [getValue()](#getValue--) | Özelliğin değerini alır. |
| [hashCode()](#hashCode--) |  |
| [isGeneratedName()](#isGeneratedName--) | Bu özellik OLE2 depolamasında bir ada sahip değilse ve yalnızca genel API için benzersiz bir ad oluşturulduysa true döndürür. |
| [isLinkedToContent()](#isLinkedToContent--) | Bu özelliğin içeriğe bağlı olup olmadığını gösterir |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setValue(Object value)](#setValue-java.lang.Object-) | Özelliğin değerini ayarlar. |
| [toBool()](#toBool--) | Özellik değerini bool olarak döndürür. |
| [toDateTime()](#toDateTime--) | Özellik değerini yerel saat diliminde DateTime olarak döndürür. |
| [toDouble()](#toDouble--) | Özellik değerini double olarak döndürür. |
| [toInt()](#toInt--) | Özellik değerini integer olarak döndürür. |
| [toString()](#toString--) | Özelliğin değerini bir dize olarak döndürür. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
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


Özelliğin adını döndürür.

**Returns:**
java.lang.String
### getSource() {#getSource--}
```
public String getSource()
```


Bağlantılı içerik kaynağı.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Özelliğin veri tipini alır.

Bakın [PropertyType](../../com.aspose.cells/propertytype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Özelliğin değerini alır.

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


Bu özellik OLE2 depolamasında bir ada sahip değilse ve yalnızca genel API için benzersiz bir ad oluşturulduysa true döndürür.

**Returns:**
boolean
### isLinkedToContent() {#isLinkedToContent--}
```
public boolean isLinkedToContent()
```


Bu özelliğin içeriğe bağlı olup olmadığını gösterir

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


Özelliğin değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

### toBool() {#toBool--}
```
public boolean toBool()
```


Özellik değerini bool olarak döndürür.

**Remarks**

Özellik türü PropertyType.Boolean değilse bir istisna fırlatır.

**Returns:**
boolean
### toDateTime() {#toDateTime--}
```
public DateTime toDateTime()
```


Özellik değerini yerel saat diliminde DateTime olarak döndürür.

**Remarks**

Özellik türü PropertyType.Date değilse bir istisna fırlatır.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### toDouble() {#toDouble--}
```
public double toDouble()
```


Özellik değerini double olarak döndürür.

**Remarks**

Özellik türü PropertyType.Float değilse bir istisna fırlatır.

**Returns:**
double
### toInt() {#toInt--}
```
public int toInt()
```


Özellik değerini integer olarak döndürür.

**Remarks**

Özellik türü PropertyType.Number değilse bir istisna fırlatır.

**Returns:**
int
### toString() {#toString--}
```
public String toString()
```


Özelliğin değerini bir dize olarak döndürür.

**Remarks**

Bir sayı özelliğini Object.ToString() kullanarak dönüştürür. Bir boolean özelliğini "Y" veya "N" olarak dönüştürür. Bir tarih özelliğini kısa tarih dizesine dönüştürür.

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

