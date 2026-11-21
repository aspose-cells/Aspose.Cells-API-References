---
title: "CommandButtonActiveXControl"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un botón de comando."
type: docs
url: /es/java/com.aspose.cells/commandbuttonactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class CommandButtonActiveXControl extends ActiveXControl
```

Representa un botón de comando.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccelerator()](#getAccelerator--) | Obtiene la tecla de acceso rápido del control. |
| [getBackOleColor()](#getBackOleColor--) | Obtiene el color ole del fondo. |
| [getCaption()](#getCaption--) | Obtiene el texto descriptivo que aparece en un control. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Obtiene los datos binarios del control. |
| [getFont()](#getFont--) | Representa la fuente del control. |
| [getForeOleColor()](#getForeOleColor--) | Obtiene el color OLE del primer plano. |
| [getHeight()](#getHeight--) | Obtiene la altura del control en unidades de puntos. |
| [getIMEMode()](#getIMEMode--) | Obtiene el modo de ejecución predeterminado del Editor de Métodos de Entrada para el control cuando recibe el foco. |
| [getLinkedCell()](#getLinkedCell--) | Obtiene la celda vinculada. |
| [getListFillRange()](#getListFillRange--) | Obtiene el rango de relleno de la lista. |
| [getMouseIcon()](#getMouseIcon--) | Obtiene un ícono personalizado para mostrar como puntero del mouse del control. |
| [getMousePointer()](#getMousePointer--) | Obtiene el tipo de ícono que se muestra como puntero del mouse del control. |
| [getPicture()](#getPicture--) | Obtiene los datos de la imagen. |
| [getPicturePosition()](#getPicturePosition--) | Obtiene la ubicación de la imagen del control relativa a su caption. |
| [getShadow()](#getShadow--) | Indica si se muestra una sombra. |
| [getTakeFocusOnClick()](#getTakeFocusOnClick--) | Indica si el control toma el foco al hacer clic. |
| [getTextAlign()](#getTextAlign--) | Representa cómo alinear el texto utilizado por el control. |
| [getType()](#getType--) | Obtiene el tipo del control ActiveX. |
| [getWidth()](#getWidth--) | Obtiene el ancho del control en unidades de puntos. |
| [getWorkbook()](#getWorkbook--) | Obtiene el objeto [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Indica si el control se redimensionará automáticamente para mostrar todo su contenido. |
| [isEnabled()](#isEnabled--) | Indica si el control puede recibir el foco y responder a eventos generados por el usuario. |
| [isLocked()](#isLocked--) | Indica si los datos en el control están bloqueados para edición. |
| [isTransparent()](#isTransparent--) | Indica si el control es transparente. |
| [isVisible()](#isVisible--) | Indica si este control es visible. |
| [isWordWrapped()](#isWordWrapped--) | Indica si el contenido del control se ajusta automáticamente al final de una línea. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccelerator(char value)](#setAccelerator-char-) | Establece la tecla de acceso rápido para el control. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indica si el control se redimensionará automáticamente para mostrar todo su contenido. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Establece el color OLE del fondo. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Establece el texto descriptivo que aparece en un control. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Indica si el control puede recibir el foco y responder a eventos generados por el usuario. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Establece el color OLE del primer plano. |
| [setHeight(double value)](#setHeight-double-) | Establece la altura del control en unidades de puntos. |
| [setIMEMode(int value)](#setIMEMode-int-) | Establece el modo de tiempo de ejecución predeterminado del Editor de Métodos de Entrada para el control cuando recibe el foco. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Establece la celda vinculada. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Establece el rango de relleno de la lista. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indica si los datos en el control están bloqueados para edición. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Establece un ícono personalizado para mostrar como puntero del ratón del control. |
| [setMousePointer(int value)](#setMousePointer-int-) | Establece el tipo de ícono que se muestra como puntero del ratón del control. |
| [setPicture(byte[] value)](#setPicture-byte---) | Establece los datos de la imagen. |
| [setPicturePosition(int value)](#setPicturePosition-int-) | Establece la ubicación de la imagen del control relativa a su caption. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indica si se muestra una sombra. |
| [setTakeFocusOnClick(boolean value)](#setTakeFocusOnClick-boolean-) | Indica si el control toma el foco al hacer clic. |
| [setTextAlign(int value)](#setTextAlign-int-) | Representa cómo alinear el texto utilizado por el control. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indica si el control es transparente. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indica si este control es visible. |
| [setWidth(double value)](#setWidth-double-) | Establece el ancho del control en unidades de puntos. |
| [setWordWrapped(boolean value)](#setWordWrapped-boolean-) | Indica si el contenido del control se ajusta automáticamente al final de una línea. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAccelerator() {#getAccelerator--}
```
public char getAccelerator()
```


Obtiene la tecla de acceso rápido del control.

**Returns:**
char
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Obtiene el color ole del fondo.

**Returns:**
int
### getCaption() {#getCaption--}
```
public String getCaption()
```


Obtiene el texto descriptivo que aparece en un control.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getData() {#getData--}
```
public byte[] getData()
```


Obtiene los datos binarios del control.

**Returns:**
byte[]
### getFont() {#getFont--}
```
public Font getFont()
```


Representa la fuente del control.

**Returns:**
[Font](../../com.aspose.cells/font)
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


Obtiene el color OLE del primer plano.

**Remarks**

No se aplica al control Image.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Obtiene la altura del control en unidades de puntos.

**Returns:**
double
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```


Obtiene el modo de ejecución predeterminado del Editor de Métodos de Entrada para el control cuando recibe el foco.

Ver [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Obtiene la celda vinculada.

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


Obtiene el rango de relleno de la lista.

**Returns:**
java.lang.String
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


Obtiene un ícono personalizado para mostrar como puntero del mouse del control.

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


Obtiene el tipo de ícono que se muestra como puntero del mouse del control.

Ver [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Returns:**
int
### getPicture() {#getPicture--}
```
public byte[] getPicture()
```


Obtiene los datos de la imagen.

**Returns:**
byte[]
### getPicturePosition() {#getPicturePosition--}
```
public int getPicturePosition()
```


Obtiene la ubicación de la imagen del control relativa a su caption.

Vea [ControlPicturePositionType](../../com.aspose.cells/controlpicturepositiontype).

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Indica si se muestra una sombra.

**Returns:**
boolean
### getTakeFocusOnClick() {#getTakeFocusOnClick--}
```
public boolean getTakeFocusOnClick()
```


Indica si el control toma el foco al hacer clic.

**Returns:**
boolean
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


Representa cómo alinear el texto utilizado por el control.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Obtiene el tipo del control ActiveX.

Ver [ControlType](../../com.aspose.cells/controltype).

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


Obtiene el ancho del control en unidades de puntos.

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Obtiene el objeto [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--).

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSize() {#isAutoSize--}
```
public boolean isAutoSize()
```


Indica si el control se redimensionará automáticamente para mostrar todo su contenido.

**Returns:**
boolean
### isEnabled() {#isEnabled--}
```
public boolean isEnabled()
```


Indica si el control puede recibir el foco y responder a eventos generados por el usuario.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Indica si los datos en el control están bloqueados para edición.

**Returns:**
boolean
### isTransparent() {#isTransparent--}
```
public boolean isTransparent()
```


Indica si el control es transparente.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Indica si este control es visible.

**Returns:**
boolean
### isWordWrapped() {#isWordWrapped--}
```
public boolean isWordWrapped()
```


Indica si el contenido del control se ajusta automáticamente al final de una línea.

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




### setAccelerator(char value) {#setAccelerator-char-}
```
public void setAccelerator(char value)
```


Establece la tecla de acceso rápido para el control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | char |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Indica si el control se redimensionará automáticamente para mostrar todo su contenido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


Establece el color OLE del fondo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Establece el texto descriptivo que aparece en un control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Indica si el control puede recibir el foco y responder a eventos generados por el usuario.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


Establece el color OLE del primer plano.

**Remarks**

No se aplica al control Image.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Establece la altura del control en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


Establece el modo de tiempo de ejecución predeterminado del Editor de Métodos de Entrada para el control cuando recibe el foco.

Ver [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Establece la celda vinculada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


Establece el rango de relleno de la lista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Indica si los datos en el control están bloqueados para edición.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


Establece un ícono personalizado para mostrar como puntero del ratón del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


Establece el tipo de ícono que se muestra como puntero del ratón del control.

Ver [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPicture(byte[] value) {#setPicture-byte---}
```
public void setPicture(byte[] value)
```


Establece los datos de la imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte[] |  |

### setPicturePosition(int value) {#setPicturePosition-int-}
```
public void setPicturePosition(int value)
```


Establece la ubicación de la imagen del control relativa a su caption.

Vea [ControlPicturePositionType](../../com.aspose.cells/controlpicturepositiontype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Indica si se muestra una sombra.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setTakeFocusOnClick(boolean value) {#setTakeFocusOnClick-boolean-}
```
public void setTakeFocusOnClick(boolean value)
```


Indica si el control toma el foco al hacer clic.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


Representa cómo alinear el texto utilizado por el control.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Indica si el control es transparente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indica si este control es visible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Establece el ancho del control en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWordWrapped(boolean value) {#setWordWrapped-boolean-}
```
public void setWordWrapped(boolean value)
```


Indica si el contenido del control se ajusta automáticamente al final de una línea.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

