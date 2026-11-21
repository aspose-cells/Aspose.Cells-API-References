---
title: "TextBoxActiveXControl"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un control ActiveX de cuadro de texto."
type: docs
url: /es/java/com.aspose.cells/textboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class TextBoxActiveXControl extends ActiveXControl
```

Representa un control ActiveX de cuadro de texto.

**Example**

```
         //Initialize a new workbook.
         Workbook book = new Workbook();
 
         //Add a TextBoxActiveXControl.
         Shape shape = book.getWorksheets().get(0).getShapes().addActiveXControl(ControlType.TEXT_BOX, 1, 0, 1, 0, 100, 50);
         TextBoxActiveXControl activeXControl = (TextBoxActiveXControl)shape.getActiveXControl();
 
         //do your business
 
         //Save the excel file.
         book.save("exmaple.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Obtiene el color ole del fondo. |
| [getBorderOleColor()](#getBorderOleColor--) | Obtiene el color ole del fondo. |
| [getBorderStyle()](#getBorderStyle--) | Obtiene el tipo de borde utilizado por el control. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Obtiene los datos binarios del control. |
| [getDropButtonStyle()](#getDropButtonStyle--) | Especifica el símbolo que se muestra en el botón desplegable |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | Especifica el comportamiento de selección al entrar en el control. |
| [getEnterKeyBehavior()](#getEnterKeyBehavior--) | Especifica el comportamiento de la tecla ENTER. |
| [getFont()](#getFont--) | Representa la fuente del control. |
| [getForeOleColor()](#getForeOleColor--) | Obtiene el color OLE del primer plano. |
| [getHeight()](#getHeight--) | Obtiene la altura del control en unidades de puntos. |
| [getHideSelection()](#getHideSelection--) | Indica si el texto seleccionado en el control aparece resaltado cuando el control no tiene el foco. |
| [getIMEMode()](#getIMEMode--) | Obtiene el modo de ejecución predeterminado del Editor de Métodos de Entrada para el control cuando recibe el foco. |
| [getIntegralHeight()](#getIntegralHeight--) | Indica si el control solo mostrará líneas completas de texto sin mostrar líneas parciales. |
| [getLinkedCell()](#getLinkedCell--) | Obtiene la celda vinculada. |
| [getListFillRange()](#getListFillRange--) | Obtiene el rango de relleno de la lista. |
| [getMaxLength()](#getMaxLength--) | Obtiene el número máximo de caracteres |
| [getMouseIcon()](#getMouseIcon--) | Obtiene un ícono personalizado para mostrar como puntero del mouse del control. |
| [getMousePointer()](#getMousePointer--) | Obtiene el tipo de ícono que se muestra como puntero del mouse del control. |
| [getPasswordChar()](#getPasswordChar--) | Obtiene un carácter que se mostrará en lugar de los caracteres ingresados. |
| [getScrollBars()](#getScrollBars--) | Indica si el control tiene barras de desplazamiento verticales, horizontales, ambas o ninguna. |
| [getShadow()](#getShadow--) | Indica si se muestra una sombra. |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | Especifica el símbolo que se muestra en el botón desplegable |
| [getSpecialEffect()](#getSpecialEffect--) | Obtiene el efecto especial del control. |
| [getTabKeyBehavior()](#getTabKeyBehavior--) | Indica si se permiten caracteres de tabulación en el texto del control. |
| [getText()](#getText--) | Obtiene el texto del control. |
| [getTextAlign()](#getTextAlign--) | Representa cómo alinear el texto utilizado por el control. |
| [getType()](#getType--) | Obtiene el tipo del control ActiveX. |
| [getWidth()](#getWidth--) | Obtiene el ancho del control en unidades de puntos. |
| [getWorkbook()](#getWorkbook--) | Obtiene el objeto [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Indica si el control se redimensionará automáticamente para mostrar todo su contenido. |
| [isAutoTab()](#isAutoTab--) | Indica si el foco se moverá automáticamente al siguiente control cuando el usuario ingrese el número máximo de caracteres. |
| [isAutoWordSelected()](#isAutoWordSelected--) | Especifica la unidad básica utilizada para ampliar una selección. |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--) | Indica si arrastrar y soltar está habilitado para el control. |
| [isEditable()](#isEditable--) | Indica si el usuario puede escribir en el control. |
| [isEnabled()](#isEnabled--) | Indica si el control puede recibir el foco y responder a eventos generados por el usuario. |
| [isLocked()](#isLocked--) | Indica si los datos en el control están bloqueados para edición. |
| [isMultiLine()](#isMultiLine--) | Indica si el control puede mostrar más de una línea de texto. |
| [isTransparent()](#isTransparent--) | Indica si el control es transparente. |
| [isVisible()](#isVisible--) | Indica si este control es visible. |
| [isWordWrapped()](#isWordWrapped--) | Indica si el contenido del control se ajusta automáticamente al final de una línea. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indica si el control se redimensionará automáticamente para mostrar todo su contenido. |
| [setAutoTab(boolean value)](#setAutoTab-boolean-) | Indica si el foco se moverá automáticamente al siguiente control cuando el usuario ingrese el número máximo de caracteres. |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) | Especifica la unidad básica utilizada para ampliar una selección. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Establece el color OLE del fondo. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Establece el color OLE del fondo. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Establece el tipo de borde utilizado por el control. |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) | Indica si arrastrar y soltar está habilitado para el control. |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) | Especifica el símbolo que se muestra en el botón desplegable |
| [setEditable(boolean value)](#setEditable-boolean-) | Indica si el usuario puede escribir en el control. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Indica si el control puede recibir el foco y responder a eventos generados por el usuario. |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) | Especifica el comportamiento de selección al entrar en el control. |
| [setEnterKeyBehavior(boolean value)](#setEnterKeyBehavior-boolean-) | Especifica el comportamiento de la tecla ENTER. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Establece el color OLE del primer plano. |
| [setHeight(double value)](#setHeight-double-) | Establece la altura del control en unidades de puntos. |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) | Indica si el texto seleccionado en el control aparece resaltado cuando el control no tiene el foco. |
| [setIMEMode(int value)](#setIMEMode-int-) | Establece el modo de tiempo de ejecución predeterminado del Editor de Métodos de Entrada para el control cuando recibe el foco. |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | Indica si el control solo mostrará líneas completas de texto sin mostrar líneas parciales. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Establece la celda vinculada. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Establece el rango de relleno de la lista. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indica si los datos en el control están bloqueados para edición. |
| [setMaxLength(int value)](#setMaxLength-int-) | Establece el número máximo de caracteres |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Establece un ícono personalizado para mostrar como puntero del ratón del control. |
| [setMousePointer(int value)](#setMousePointer-int-) | Establece el tipo de ícono que se muestra como puntero del ratón del control. |
| [setMultiLine(boolean value)](#setMultiLine-boolean-) | Indica si el control puede mostrar más de una línea de texto. |
| [setPasswordChar(char value)](#setPasswordChar-char-) | Establece un carácter que se mostrará en lugar de los caracteres ingresados. |
| [setScrollBars(int value)](#setScrollBars-int-) | Indica si el control tiene barras de desplazamiento verticales, horizontales, ambas o ninguna. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indica si se muestra una sombra. |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) | Especifica el símbolo que se muestra en el botón desplegable |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Establece el efecto especial del control. |
| [setTabKeyBehavior(boolean value)](#setTabKeyBehavior-boolean-) | Indica si se permiten caracteres de tabulación en el texto del control. |
| [setText(String value)](#setText-java.lang.String-) | Establece el texto del control. |
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

**Example**

```
         //excel default color system 12 or green(0x0000FF00)
         activeXControl.setBorderOleColor(/*unchecked*/((int)0x80000012L));
```

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Obtiene el tipo de borde utilizado por el control.

Ver [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Example**

```
         activeXControl.setBorderStyle(com.aspose.cells.ControlBorderType.SINGLE);
```

**Returns:**
int
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
### getDropButtonStyle() {#getDropButtonStyle--}
```
public int getDropButtonStyle()
```


Especifica el símbolo que se muestra en el botón desplegable

Ver [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Example**

```
         activeXControl.setDropButtonStyle(com.aspose.cells.DropButtonStyle.ARROW);
```

**Returns:**
int
### getEnterFieldBehavior() {#getEnterFieldBehavior--}
```
public boolean getEnterFieldBehavior()
```


Especifica el comportamiento de selección al entrar en el control. True indica que la selección permanece sin cambios desde la última vez que el control estuvo activo. False indica que todo el texto del control se seleccionará al entrar en el control.

**Example**

```
         if(!activeXControl.getEnterFieldBehavior())
         {
             activeXControl.setEnterFieldBehavior(true);
         }
```

**Returns:**
boolean
### getEnterKeyBehavior() {#getEnterKeyBehavior--}
```
public boolean getEnterKeyBehavior()
```


Especifica el comportamiento de la tecla ENTER. Verdadero indica que al presionar ENTER se creará una nueva línea. Falso indica que al presionar ENTER el foco se moverá al siguiente objeto en el orden de tabulación.

**Example**

```
         if(!activeXControl.getEnterKeyBehavior())
         {
             activeXControl.setEnterKeyBehavior(true);
         }
```

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

**Example**

```
         if(!activeXControl.getHideSelection())
         {
             activeXControl.setHideSelection(true);
         }
```

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
### getIntegralHeight() {#getIntegralHeight--}
```
public boolean getIntegralHeight()
```


Indica si el control solo mostrará líneas completas de texto sin mostrar líneas parciales.

**Example**

```
         if(!activeXControl.getIntegralHeight())
         {
             activeXControl.setIntegralHeight(true);
         }
```

**Returns:**
boolean
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
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Obtiene el número máximo de caracteres

**Example**

```
         if(activeXControl.getMaxLength() == 0)
         {
             activeXControl.setMaxLength(30);
         }
```

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
### getPasswordChar() {#getPasswordChar--}
```
public char getPasswordChar()
```


Obtiene un carácter que se mostrará en lugar de los caracteres ingresados.

**Example**

```
         activeXControl.setPasswordChar('a');
```

**Returns:**
char
### getScrollBars() {#getScrollBars--}
```
public int getScrollBars()
```


Indica si el control tiene barras de desplazamiento verticales, horizontales, ambas o ninguna.

Ver [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Example**

```
         activeXControl.setScrollBars(com.aspose.cells.ControlScrollBarType.BARS_VERTICAL);
```

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Indica si se muestra una sombra.

**Returns:**
boolean
### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}
```
public int getShowDropButtonTypeWhen()
```


Especifica el símbolo que se muestra en el botón desplegable

Ver [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Example**

```
         activeXControl.setShowDropButtonTypeWhen(com.aspose.cells.ShowDropButtonType.FOCUS);
```

**Returns:**
int
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


Obtiene el efecto especial del control.

Ver [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Example**

```
         activeXControl.setSpecialEffect(com.aspose.cells.ControlSpecialEffectType.BUMP);
```

**Returns:**
int
### getTabKeyBehavior() {#getTabKeyBehavior--}
```
public boolean getTabKeyBehavior()
```


Indica si se permiten caracteres de tabulación en el texto del control.

**Example**

```
         if(!activeXControl.getTabKeyBehavior())
         {
             activeXControl.setTabKeyBehavior(true);
         }
```

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Obtiene el texto del control.

**Example**

```
         activeXControl.setText("This is a test.");
```

**Returns:**
java.lang.String
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

**Example**

```
         /*Aspose.Cells.Drawing.ActiveXControls.ControlType*/int type = activeXControl.getType();
```

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
### isAutoTab() {#isAutoTab--}
```
public boolean isAutoTab()
```


Indica si el foco se moverá automáticamente al siguiente control cuando el usuario ingrese el número máximo de caracteres.

**Example**

```
         if(!activeXControl.isAutoTab())
         {
             activeXControl.setAutoTab(true);
         }
```

**Returns:**
boolean
### isAutoWordSelected() {#isAutoWordSelected--}
```
public boolean isAutoWordSelected()
```


Especifica la unidad básica utilizada para ampliar una selección. True indica que la unidad básica es un solo carácter. false indica que la unidad básica es una palabra completa.

**Example**

```
         if(!activeXControl.isAutoWordSelected())
         {
             activeXControl.setAutoWordSelected(true);
         }
```

**Returns:**
boolean
### isDragBehaviorEnabled() {#isDragBehaviorEnabled--}
```
public boolean isDragBehaviorEnabled()
```


Indica si arrastrar y soltar está habilitado para el control.

**Example**

```
         if(!activeXControl.isDragBehaviorEnabled())
         {
             activeXControl.setDragBehaviorEnabled(true);
         }
```

**Returns:**
boolean
### isEditable() {#isEditable--}
```
public boolean isEditable()
```


Indica si el usuario puede escribir en el control.

**Example**

```
         if(!activeXControl.isEditable())
         {
             activeXControl.setEditable(true);
         }
```

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
### isMultiLine() {#isMultiLine--}
```
public boolean isMultiLine()
```


Indica si el control puede mostrar más de una línea de texto.

**Example**

```
         if(!activeXControl.isMultiLine())
         {
             activeXControl.setMultiLine(true);
         }
```

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

**Example**

```
         if(!activeXControl.isWordWrapped())
         {
             activeXControl.setWordWrapped(true);
         }
```

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

### setAutoTab(boolean value) {#setAutoTab-boolean-}
```
public void setAutoTab(boolean value)
```


Indica si el foco se moverá automáticamente al siguiente control cuando el usuario ingrese el número máximo de caracteres.

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

### setEnterKeyBehavior(boolean value) {#setEnterKeyBehavior-boolean-}
```
public void setEnterKeyBehavior(boolean value)
```


Especifica el comportamiento de la tecla ENTER. Verdadero indica que al presionar ENTER se creará una nueva línea. Falso indica que al presionar ENTER el foco se moverá al siguiente objeto en el orden de tabulación.

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

### setIntegralHeight(boolean value) {#setIntegralHeight-boolean-}
```
public void setIntegralHeight(boolean value)
```


Indica si el control solo mostrará líneas completas de texto sin mostrar líneas parciales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

### setMultiLine(boolean value) {#setMultiLine-boolean-}
```
public void setMultiLine(boolean value)
```


Indica si el control puede mostrar más de una línea de texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPasswordChar(char value) {#setPasswordChar-char-}
```
public void setPasswordChar(char value)
```


Establece un carácter que se mostrará en lugar de los caracteres ingresados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | char |  |

### setScrollBars(int value) {#setScrollBars-int-}
```
public void setScrollBars(int value)
```


Indica si el control tiene barras de desplazamiento verticales, horizontales, ambas o ninguna.

Ver [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

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

### setTabKeyBehavior(boolean value) {#setTabKeyBehavior-boolean-}
```
public void setTabKeyBehavior(boolean value)
```


Indica si se permiten caracteres de tabulación en el texto del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Establece el texto del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

