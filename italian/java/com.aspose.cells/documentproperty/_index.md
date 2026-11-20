---
title: "DocumentProperty"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta una proprietà del documento personalizzata o predefinita."
type: docs
url: /it/java/com.aspose.cells/documentproperty/
---

**Inheritance:**
java.lang.Object
```
public class DocumentProperty
```

Rappresenta una proprietà del documento personalizzata o predefinita.

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Restituisce il nome della proprietà. |
| [getSource()](#getSource--) | La fonte del contenuto collegato. |
| [getType()](#getType--) | Restituisce il tipo di dati della proprietà. |
| [getValue()](#getValue--) | Restituisce il valore della proprietà. |
| [hashCode()](#hashCode--) |  |
| [isGeneratedName()](#isGeneratedName--) | Restituisce true se questa proprietà non ha un nome nello storage OLE2 ed è stato generato un nome univoco solo per l'API pubblica. |
| [isLinkedToContent()](#isLinkedToContent--) | Indica se questa proprietà è collegata al contenuto |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setValue(Object value)](#setValue-java.lang.Object-) | Imposta il valore della proprietà. |
| [toBool()](#toBool--) | Restituisce il valore della proprietà come bool. |
| [toDateTime()](#toDateTime--) | Restituisce il valore della proprietà come DateTime nel fuso orario locale. |
| [toDouble()](#toDouble--) | Restituisce il valore della proprietà come double. |
| [toInt()](#toInt--) | Restituisce il valore della proprietà come integer. |
| [toString()](#toString--) | Restituisce il valore della proprietà come stringa. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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


Restituisce il nome della proprietà.

**Returns:**
java.lang.String
### getSource() {#getSource--}
```
public String getSource()
```


La fonte del contenuto collegato.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Restituisce il tipo di dati della proprietà.

Vedi [PropertyType](../../com.aspose.cells/propertytype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Restituisce il valore della proprietà.

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


Restituisce true se questa proprietà non ha un nome nello storage OLE2 ed è stato generato un nome univoco solo per l'API pubblica.

**Returns:**
boolean
### isLinkedToContent() {#isLinkedToContent--}
```
public boolean isLinkedToContent()
```


Indica se questa proprietà è collegata al contenuto

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


Imposta il valore della proprietà.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

### toBool() {#toBool--}
```
public boolean toBool()
```


Restituisce il valore della proprietà come bool.

**Remarks**

Genera un'eccezione se il tipo di proprietà non è PropertyType.Boolean.

**Returns:**
boolean
### toDateTime() {#toDateTime--}
```
public DateTime toDateTime()
```


Restituisce il valore della proprietà come DateTime nel fuso orario locale.

**Remarks**

Genera un'eccezione se il tipo di proprietà non è PropertyType.Date.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### toDouble() {#toDouble--}
```
public double toDouble()
```


Restituisce il valore della proprietà come double.

**Remarks**

Genera un'eccezione se il tipo di proprietà non è PropertyType.Float.

**Returns:**
double
### toInt() {#toInt--}
```
public int toInt()
```


Restituisce il valore della proprietà come integer.

**Remarks**

Genera un'eccezione se il tipo di proprietà non è PropertyType.Number.

**Returns:**
int
### toString() {#toString--}
```
public String toString()
```


Restituisce il valore della proprietà come stringa.

**Remarks**

Converte una proprietà numerica usando Object.ToString(). Converte una proprietà booleana in "Y" o "N". Converte una proprietà data in una stringa di data breve.

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

