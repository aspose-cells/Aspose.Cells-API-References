---
title: "Hipervínculo"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa un hipervínculo."
type: docs
url: /es/java/com.aspose.cells/hyperlink/
---

**Inheritance:**
java.lang.Object
```
public class Hyperlink
```

Encapsula el objeto que representa un hipervínculo.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Workbook object
         workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a hyperlink to a URL at "A1" cell
         int index = worksheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
         //Getting a Hyperlink by index.
         Hyperlink hyperlink = worksheet.getHyperlinks().get(index);
         //Setting display text of this hyperlink.
         hyperlink.setTextToDisplay("Aspose");
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [delete()](#delete--) | Elimina este hipervínculo. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddress()](#getAddress--) | Representa la dirección de un hipervínculo. |
| [getArea()](#getArea--) | Obtiene el rango del hipervínculo. |
| [getClass()](#getClass--) |  |
| [getLinkType()](#getLinkType--) | Obtiene el tipo de enlace. |
| [getScreenTip()](#getScreenTip--) | Devuelve o establece el texto de ScreenTip para el hipervínculo especificado. |
| [getTextToDisplay()](#getTextToDisplay--) | Representa el texto que se mostrará para el hipervínculo especificado. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddress(String value)](#setAddress-java.lang.String-) | Representa la dirección de un hipervínculo. |
| [setScreenTip(String value)](#setScreenTip-java.lang.String-) | Devuelve o establece el texto de ScreenTip para el hipervínculo especificado. |
| [setTextToDisplay(String value)](#setTextToDisplay-java.lang.String-) | Representa el texto que se mostrará para el hipervínculo especificado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### delete() {#delete--}
```
public void delete()
```


Elimina este hipervínculo.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAddress() {#getAddress--}
```
public String getAddress()
```


Representa la dirección de un hipervínculo.

**Returns:**
java.lang.String
### getArea() {#getArea--}
```
public CellArea getArea()
```


Obtiene el rango del hipervínculo.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getLinkType() {#getLinkType--}
```
public int getLinkType()
```


Obtiene el tipo de enlace.

Ver [TargetModeType](../../com.aspose.cells/targetmodetype).

**Returns:**
int
### getScreenTip() {#getScreenTip--}
```
public String getScreenTip()
```


Devuelve o establece el texto de ScreenTip para el hipervínculo especificado.

**Returns:**
java.lang.String
### getTextToDisplay() {#getTextToDisplay--}
```
public String getTextToDisplay()
```


Representa el texto que se mostrará para el hipervínculo especificado. El valor predeterminado es la dirección del hipervínculo.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAddress(String value) {#setAddress-java.lang.String-}
```
public void setAddress(String value)
```


Representa la dirección de un hipervínculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setScreenTip(String value) {#setScreenTip-java.lang.String-}
```
public void setScreenTip(String value)
```


Devuelve o establece el texto de ScreenTip para el hipervínculo especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTextToDisplay(String value) {#setTextToDisplay-java.lang.String-}
```
public void setTextToDisplay(String value)
```


Representa el texto que se mostrará para el hipervínculo especificado. El valor predeterminado es la dirección del hipervínculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

