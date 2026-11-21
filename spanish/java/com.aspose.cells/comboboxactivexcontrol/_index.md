---
title: "ComboBoxActiveXControl"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un control ActiveX ComboBox."
type: docs
url: /es/java/com.aspose.cells/comboboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class ComboBoxActiveXControl extends ActiveXControl
```

Representa un control ActiveX ComboBox.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Obtiene el color ole del fondo. |
| [getBorderOleColor()](#getBorderOleColor--) | Obtiene el color ole del fondo. |
| [getBorderStyle()](#getBorderStyle--) | Obtiene el tipo de borde utilizado por el control. |
| [getBoundColumn()](#getBoundColumn--) | Representa cómo se determina la propiedad Value para un ComboBox o ListBox cuando el valor de la propiedad MultiSelect es (fmMultiSelectSingle). |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Representa el número de columnas a mostrar en un ComboBox o ListBox. |
| [getColumnWidths()](#getColumnWidths--) | Obtiene el ancho de la columna. |
| [getData()](#getData--) | Obtiene los datos binarios del control. |
| [getDropButtonStyle()](#getDropButtonStyle--) | Especifica el símbolo que se muestra en el botón desplegable |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | Especifica el comportamiento de selección al entrar en el control. |
| [getFont()](#getFont--) | Representa la fuente del control. |
| [getForeOleColor()](#getForeOleColor--) | Obtiene el color OLE del primer plano. |
| [getHeight()](#getHeight--) | Obtiene la altura del control en unidades de puntos. |
| [getHideSelection()](#getHideSelection--) | Indica si el texto seleccionado en el control aparece resaltado cuando el control no tiene el foco. |
| [getIMEMode()](#getIMEMode--) | Obtiene el modo de ejecución predeterminado del Editor de Métodos de Entrada para el control cuando recibe el foco. |
| [getLinkedCell()](#getLinkedCell--) | Obtiene la celda vinculada. |
| [getListFillRange()](#getListFillRange--) | Obtiene el rango de relleno de la lista. |
| [getListRows()](#getListRows--) | Representa el número máximo de filas a mostrar en la lista. |
| [getListStyle()](#getListStyle--) | Obtiene la apariencia visual. |
| [getListWidth()](#getListWidth--) | Obtiene el ancho en unidades de puntos. |
| [getMatchEntry()](#getMatchEntry--) | Indica cómo un ListBox o ComboBox busca en su lista mientras el usuario escribe. |
| [getMaxLength()](#getMaxLength--) | Obtiene el número máximo de caracteres |
| [getMouseIcon()](#getMouseIcon--) | Obtiene un ícono personalizado para mostrar como puntero del mouse del control. |
| [getMousePointer()](#getMousePointer--) | Obtiene el tipo de ícono que se muestra como puntero del mouse del control. |
| [getSelectionMargin()](#getSelectionMargin--) | Indica si el usuario puede seleccionar una línea de texto haciendo clic en la zona a la izquierda del texto. |
| [getShadow()](#getShadow--) | Indica si se muestra una sombra. |
| [getShowColumnHeads()](#getShowColumnHeads--) | Indica si se muestran los encabezados de columna. |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | Especifica el símbolo que se muestra en el botón desplegable |
| [getSpecialEffect()](#getSpecialEffect--) | Obtiene el efecto especial del control. |
| [getTextAlign()](#getTextAlign--) | Representa cómo alinear el texto utilizado por el control. |
| [getTextColumn()](#getTextColumn--) | Representa la columna en un ComboBox o ListBox que se muestra al usuario. |
| [getType()](#getType--) | Obtiene el tipo del control ActiveX. |
| [getValue()](#getValue--) | Obtiene el valor del control. |
| [getWidth()](#getWidth--) | Obtiene el ancho del control en unidades de puntos. |
| [getWorkbook()](#getWorkbook--) | Obtiene el objeto [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Indica si el control se redimensionará automáticamente para mostrar todo su contenido. |
| [isAutoWordSelected()](#isAutoWordSelected--) | Especifica la unidad básica utilizada para ampliar una selección. |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--) | Indica si arrastrar y soltar está habilitado para el control. |
| [isEditable()](#isEditable--) | Indica si el usuario puede escribir en el control. |
| [isEnabled()](#isEnabled--) | Indica si el control puede recibir el foco y responder a eventos generados por el usuario. |
| [isLocked()](#isLocked--) | Indica si los datos en el control están bloqueados para edición. |
| [isTransparent()](#isTransparent--) | Indica si el control es transparente. |
| [isVisible()](#isVisible--) | Indica si este control es visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indica si el control se redimensionará automáticamente para mostrar todo su contenido. |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) | Especifica la unidad básica utilizada para ampliar una selección. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Establece el color OLE del fondo. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Establece el color OLE del fondo. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Establece el tipo de borde utilizado por el control. |
| [setBoundColumn(int value)](#setBoundColumn-int-) | Representa cómo se determina la propiedad Value para un ComboBox o ListBox cuando el valor de la propiedad MultiSelect es (fmMultiSelectSingle). |
| [setColumnCount(int value)](#setColumnCount-int-) | Representa el número de columnas a mostrar en un ComboBox o ListBox. |
| [setColumnWidths(double value)](#setColumnWidths-double-) | Establece el ancho de la columna. |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) | Indica si arrastrar y soltar está habilitado para el control. |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) | Especifica el símbolo que se muestra en el botón desplegable |
| [setEditable(boolean value)](#setEditable-boolean-) | Indica si el usuario puede escribir en el control. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Indica si el control puede recibir el foco y responder a eventos generados por el usuario. |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) | Especifica el comportamiento de selección al entrar en el control. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Establece el color OLE del primer plano. |
| [setHeight(double value)](#setHeight-double-) | Establece la altura del control en unidades de puntos. |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) | Indica si el texto seleccionado en el control aparece resaltado cuando el control no tiene el foco. |
| [setIMEMode(int value)](#setIMEMode-int-) | Establece el modo de tiempo de ejecución predeterminado del Editor de Métodos de Entrada para el control cuando recibe el foco. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Establece la celda vinculada. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Establece el rango de relleno de la lista. |
| [setListRows(int value)](#setListRows-int-) | Representa el número máximo de filas a mostrar en la lista. |
| [setListStyle(int value)](#setListStyle-int-) | Establece la apariencia visual. |
| [setListWidth(double value)](#setListWidth-double-) | Establece el ancho en unidades de puntos. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indica si los datos en el control están bloqueados para edición. |
| [setMatchEntry(int value)](#setMatchEntry-int-) | Indica cómo un ListBox o ComboBox busca en su lista mientras el usuario escribe. |
| [setMaxLength(int value)](#setMaxLength-int-) | Establece el número máximo de caracteres |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Establece un ícono personalizado para mostrar como puntero del ratón del control. |
| [setMousePointer(int value)](#setMousePointer-int-) | Establece el tipo de ícono que se muestra como puntero del ratón del control. |
| [setSelectionMargin(boolean value)](#setSelectionMargin-boolean-) | Indica si el usuario puede seleccionar una línea de texto haciendo clic en la zona a la izquierda del texto. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indica si se muestra una sombra. |
| [setShowColumnHeads(boolean value)](#setShowColumnHeads-boolean-) | Indica si se muestran los encabezados de columna. |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) | Especifica el símbolo que se muestra en el botón desplegable |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Establece el efecto especial del control. |
| [setTextAlign(int value)](#setTextAlign-int-) | Representa cómo alinear el texto utilizado por el control. |
| [setTextColumn(int value)](#setTextColumn-int-) | Representa la columna en un ComboBox o ListBox que se muestra al usuario. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indica si el control es transparente. |
| [setValue(String value)](#setValue-java.lang.String-) | Establece el valor del control. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indica si este control es visible. |
| [setWidth(double value)](#setWidth-double-) | Establece el ancho del control en unidades de puntos. |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Obtiene el color ole del fondo.

**Returns:**
int
### getBorderOleColor() {#getBorderOleColor--}
```
public int getBorderOleColor()
```


Obtiene el color ole del fondo.

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Obtiene el tipo de borde utilizado por el control.

Ver [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Returns:**
int
### getBoundColumn() {#getBoundColumn--}
```
public int getBoundColumn()
```


Representa cómo se determina la propiedad Value para un ComboBox o ListBox cuando el valor de la propiedad MultiSelect es (fmMultiSelectSingle).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Representa el número de columnas a mostrar en un ComboBox o ListBox.

**Returns:**
int
### getColumnWidths() {#getColumnWidths--}
```
public double getColumnWidths()
```


Obtiene el ancho de la columna.

**Returns:**
double
### getData() {#getData--}
```
public byte[] getData()
```


Obtiene los datos binarios del control.

**Returns:**
byte[]
### getDropButtonStyle() {#getDropButtonStyle--}
```
public int getDropButtonStyle()
```


Especifica el símbolo que se muestra en el botón desplegable

Ver [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Returns:**
int
### getEnterFieldBehavior() {#getEnterFieldBehavior--}
```
public boolean getEnterFieldBehavior()
```


Especifica el comportamiento de selección al entrar en el control. True indica que la selección permanece sin cambios desde la última vez que el control estuvo activo. False indica que todo el texto del control se seleccionará al entrar en el control.

**Returns:**
boolean
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
### getHideSelection() {#getHideSelection--}
```
public boolean getHideSelection()
```


Indica si el texto seleccionado en el control aparece resaltado cuando el control no tiene el foco.

**Returns:**
boolean
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
### getListRows() {#getListRows--}
```
public int getListRows()
```


Representa el número máximo de filas a mostrar en la lista.

**Returns:**
int
### getListStyle() {#getListStyle--}
```
public int getListStyle()
```


Obtiene la apariencia visual.

Ver [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Returns:**
int
### getListWidth() {#getListWidth--}
```
public double getListWidth()
```


Obtiene el ancho en unidades de puntos.

**Returns:**
double
### getMatchEntry() {#getMatchEntry--}
```
public int getMatchEntry()
```


Indica cómo un ListBox o ComboBox busca en su lista mientras el usuario escribe.

Ver [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

**Returns:**
int
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Obtiene el número máximo de caracteres

**Returns:**
int
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
### getSelectionMargin() {#getSelectionMargin--}
```
public boolean getSelectionMargin()
```


Indica si el usuario puede seleccionar una línea de texto haciendo clic en la zona a la izquierda del texto.

**Returns:**
boolean
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Indica si se muestra una sombra.

**Returns:**
boolean
### getShowColumnHeads() {#getShowColumnHeads--}
```
public boolean getShowColumnHeads()
```


Indica si se muestran los encabezados de columna.

**Returns:**
boolean
### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}
```
public int getShowDropButtonTypeWhen()
```


Especifica el símbolo que se muestra en el botón desplegable

Ver [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Returns:**
int
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


Obtiene el efecto especial del control.

Ver [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Returns:**
int
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


Representa cómo alinear el texto utilizado por el control.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextColumn() {#getTextColumn--}
```
public int getTextColumn()
```


Representa la columna en un ComboBox o ListBox que se muestra al usuario.

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
### getValue() {#getValue--}
```
public String getValue()
```


Obtiene el valor del control.

**Returns:**
java.lang.String
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
### isAutoWordSelected() {#isAutoWordSelected--}
```
public boolean isAutoWordSelected()
```


Especifica la unidad básica utilizada para ampliar una selección. True indica que la unidad básica es un solo carácter. false indica que la unidad básica es una palabra completa.

**Returns:**
boolean
### isDragBehaviorEnabled() {#isDragBehaviorEnabled--}
```
public boolean isDragBehaviorEnabled()
```


Indica si arrastrar y soltar está habilitado para el control.

**Returns:**
boolean
### isEditable() {#isEditable--}
```
public boolean isEditable()
```


Indica si el usuario puede escribir en el control.

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
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Indica si el control se redimensionará automáticamente para mostrar todo su contenido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutoWordSelected(boolean value) {#setAutoWordSelected-boolean-}
```
public void setAutoWordSelected(boolean value)
```


Especifica la unidad básica utilizada para ampliar una selección. True indica que la unidad básica es un solo carácter. false indica que la unidad básica es una palabra completa.

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

### setBorderOleColor(int value) {#setBorderOleColor-int-}
```
public void setBorderOleColor(int value)
```


Establece el color OLE del fondo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Establece el tipo de borde utilizado por el control.

Ver [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBoundColumn(int value) {#setBoundColumn-int-}
```
public void setBoundColumn(int value)
```


Representa cómo se determina la propiedad Value para un ComboBox o ListBox cuando el valor de la propiedad MultiSelect es (fmMultiSelectSingle).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setColumnCount(int value) {#setColumnCount-int-}
```
public void setColumnCount(int value)
```


Representa el número de columnas a mostrar en un ComboBox o ListBox.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setColumnWidths(double value) {#setColumnWidths-double-}
```
public void setColumnWidths(double value)
```


Establece el ancho de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setDragBehaviorEnabled(boolean value) {#setDragBehaviorEnabled-boolean-}
```
public void setDragBehaviorEnabled(boolean value)
```


Indica si arrastrar y soltar está habilitado para el control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDropButtonStyle(int value) {#setDropButtonStyle-int-}
```
public void setDropButtonStyle(int value)
```


Especifica el símbolo que se muestra en el botón desplegable

Ver [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setEditable(boolean value) {#setEditable-boolean-}
```
public void setEditable(boolean value)
```


Indica si el usuario puede escribir en el control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Indica si el control puede recibir el foco y responder a eventos generados por el usuario.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnterFieldBehavior(boolean value) {#setEnterFieldBehavior-boolean-}
```
public void setEnterFieldBehavior(boolean value)
```


Especifica el comportamiento de selección al entrar en el control. True indica que la selección permanece sin cambios desde la última vez que el control estuvo activo. False indica que todo el texto del control se seleccionará al entrar en el control.

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

### setHideSelection(boolean value) {#setHideSelection-boolean-}
```
public void setHideSelection(boolean value)
```


Indica si el texto seleccionado en el control aparece resaltado cuando el control no tiene el foco.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

### setListRows(int value) {#setListRows-int-}
```
public void setListRows(int value)
```


Representa el número máximo de filas a mostrar en la lista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setListStyle(int value) {#setListStyle-int-}
```
public void setListStyle(int value)
```


Establece la apariencia visual.

Ver [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setListWidth(double value) {#setListWidth-double-}
```
public void setListWidth(double value)
```


Establece el ancho en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Indica si los datos en el control están bloqueados para edición.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMatchEntry(int value) {#setMatchEntry-int-}
```
public void setMatchEntry(int value)
```


Indica cómo un ListBox o ComboBox busca en su lista mientras el usuario escribe.

Ver [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


Establece el número máximo de caracteres

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

### setSelectionMargin(boolean value) {#setSelectionMargin-boolean-}
```
public void setSelectionMargin(boolean value)
```


Indica si el usuario puede seleccionar una línea de texto haciendo clic en la zona a la izquierda del texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Indica si se muestra una sombra.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowColumnHeads(boolean value) {#setShowColumnHeads-boolean-}
```
public void setShowColumnHeads(boolean value)
```


Indica si se muestran los encabezados de columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowDropButtonTypeWhen(int value) {#setShowDropButtonTypeWhen-int-}
```
public void setShowDropButtonTypeWhen(int value)
```


Especifica el símbolo que se muestra en el botón desplegable

Ver [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```


Establece el efecto especial del control.

Ver [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

### setTextColumn(int value) {#setTextColumn-int-}
```
public void setTextColumn(int value)
```


Representa la columna en un ComboBox o ListBox que se muestra al usuario.

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

### setValue(String value) {#setValue-java.lang.String-}
```
public void setValue(String value)
```


Establece el valor del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

