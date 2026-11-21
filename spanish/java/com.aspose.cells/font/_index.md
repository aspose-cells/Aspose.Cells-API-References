---
title: "Font"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto de fuente usado en una hoja de cálculo."
type: docs
url: /es/java/com.aspose.cells/font/
---

**Inheritance:**
java.lang.Object
```
public class Font
```

Encapsula el objeto de fuente usado en una hoja de cálculo.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Hello Aspose!");
 
         Font font = cell.getStyle().getFont();
 
         //Setting the font name to "Times New Roman"
         font.setName("Times New Roman");
 
         //Setting font size to 14
         font.setSize(14);
 
         //setting font color as Red
         font.setColor(com.aspose.cells.Color.getRed());           
 
         //Saving the Excel file
         workbook.save("dest.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | Comprueba si dos fuentes son iguales. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Obtiene el color con un valor ARGB de 32 bits. |
| [getCapsType()](#getCapsType--) | Obtiene el tipo de mayúsculas del texto. |
| [getCharset()](#getCharset--) | Representa el conjunto de caracteres. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Obtiene el [Color](../../com.aspose.cells/color) de la fuente. |
| [getDoubleSize()](#getDoubleSize--) | Obtiene el tamaño doble de la fuente. |
| [getName()](#getName--) | Obtiene el nombre de la [Font](../../com.aspose.cells/font). |
| [getSchemeType()](#getSchemeType--) | Obtiene el tipo de esquema de la fuente. |
| [getScriptOffset()](#getScriptOffset--) | Obtiene el desplazamiento del script, en unidades de porcentaje |
| [getSize()](#getSize--) | Obtiene el tamaño de la fuente. |
| [getStrikeType()](#getStrikeType--) | Obtiene el tipo de tachado del texto. |
| [getThemeColor()](#getThemeColor--) | Obtiene el color del tema. |
| [getUnderline()](#getUnderline--) | Obtiene el tipo de subrayado de la fuente. |
| [hashCode()](#hashCode--) |  |
| [isBold()](#isBold--) | Obtiene un valor que indica si la fuente está en negrita. |
| [isItalic()](#isItalic--) | Obtiene un valor que indica si la fuente está en cursiva. |
| [isNormalizeHeights()](#isNormalizeHeights--) | Indica si la normalización de altura debe aplicarse a la ejecución de texto. |
| [isStrikeout()](#isStrikeout--) | Obtiene un valor que indica si la fuente tiene tachado simple. |
| [isSubscript()](#isSubscript--) | Obtiene un valor que indica si la fuente está en subíndice. |
| [isSuperscript()](#isSuperscript--) | Obtiene un valor que indica si la fuente está en superíndice. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | Establece el color con un valor ARGB de 32 bits. |
| [setBold(boolean value)](#setBold-boolean-) | Establece un valor que indica si la fuente está en negrita. |
| [setCapsType(int value)](#setCapsType-int-) | Establece el tipo de mayúsculas del texto. |
| [setCharset(int value)](#setCharset-int-) | Representa el conjunto de caracteres. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Establece el [Color](../../com.aspose.cells/color) de la fuente. |
| [setDoubleSize(double value)](#setDoubleSize-double-) | Establece el doble tamaño de la fuente. |
| [setItalic(boolean value)](#setItalic-boolean-) | Establece un valor que indica si la fuente está en cursiva. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre de la [Font](../../com.aspose.cells/font). |
| [setName(String name, int type)](#setName-java.lang.String-int-) | Establece el nombre y el esquema de la fuente. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | Indica si la normalización de altura debe aplicarse a la ejecución de texto. |
| [setSchemeType(int value)](#setSchemeType-int-) | Establece el tipo de esquema de la fuente. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | Establece el desplazamiento del script, en unidades de porcentaje. |
| [setSize(int value)](#setSize-int-) | Establece el tamaño de la fuente. |
| [setStrikeType(int value)](#setStrikeType-int-) | Obtiene el tipo de tachado del texto. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | Establece un valor que indica si la fuente tiene un tachado simple. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | Establece un valor que indica si la fuente está en subíndice. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | Establece un valor que indica si la fuente está en superíndice. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Establece el color del tema. |
| [setUnderline(int value)](#setUnderline-int-) | Establece el tipo de subrayado de la fuente. |
| [toString()](#toString--) | Devuelve una cadena que representa el objeto Cell actual. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Font font) {#equals-com.aspose.cells.Font-}
```
public boolean equals(Font font)
```


Comprueba si dos fuentes son iguales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| font | [Font](../../com.aspose.cells/font) | Objeto de fuente comparado. |

**Returns:**
booleano - Verdadero si es igual al objeto de fuente comparado.
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
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


Obtiene el color con un valor ARGB de 32 bits.

**Returns:**
int
### getCapsType() {#getCapsType--}
```
public int getCapsType()
```


Obtiene el tipo de mayúsculas del texto.

Ver [TextCapsType](../../com.aspose.cells/textcapstype).

**Remarks**

Solo para las fuentes de Shapes o Charts. NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--). Esta propiedad será eliminada 12 meses después, a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getCharset() {#getCharset--}
```
public int getCharset()
```


Representa el conjunto de caracteres.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


Obtiene el [Color](../../com.aspose.cells/color) de la fuente.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDoubleSize() {#getDoubleSize--}
```
public double getDoubleSize()
```


Obtiene el tamaño doble de la fuente.

**Returns:**
double
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre de la [Font](../../com.aspose.cells/font).

**Remarks**

Si esta propiedad se usa para establecer el nombre de la fuente, el [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) se actualizará a [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE).

**Returns:**
java.lang.String
### getSchemeType() {#getSchemeType--}
```
public int getSchemeType()
```


Obtiene el tipo de esquema de la fuente.

Ver [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Returns:**
int
### getScriptOffset() {#getScriptOffset--}
```
public double getScriptOffset()
```


Obtiene el desplazamiento del script, en unidades de porcentaje

**Remarks**

Solo para formas y gráficos.

**Returns:**
double
### getSize() {#getSize--}
```
public int getSize()
```


Obtiene el tamaño de la fuente.

**Returns:**
int
### getStrikeType() {#getStrikeType--}
```
public int getStrikeType()
```


Obtiene el tipo de tachado del texto.

Ver [TextStrikeType](../../com.aspose.cells/textstriketype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Obtiene el color del tema.

**Remarks**

Si el color de la fuente no es un color de tema, se devolverá NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getUnderline() {#getUnderline--}
```
public int getUnderline()
```


Obtiene el tipo de subrayado de la fuente.

Ver [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBold() {#isBold--}
```
public boolean isBold()
```


Obtiene un valor que indica si la fuente está en negrita.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Obtiene un valor que indica si la fuente está en cursiva.

**Returns:**
boolean
### isNormalizeHeights() {#isNormalizeHeights--}
```
public boolean isNormalizeHeights()
```


Indica si la normalización de altura debe aplicarse a la ejecución de texto.

**Remarks**

Solo para las fuentes de Shapes o Charts. NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--). Esta propiedad será eliminada 12 meses después, a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### isStrikeout() {#isStrikeout--}
```
public boolean isStrikeout()
```


Obtiene un valor que indica si la fuente tiene tachado simple.

**Returns:**
boolean
### isSubscript() {#isSubscript--}
```
public boolean isSubscript()
```


Obtiene un valor que indica si la fuente está en subíndice.

**Returns:**
boolean
### isSuperscript() {#isSuperscript--}
```
public boolean isSuperscript()
```


Obtiene un valor que indica si la fuente está en superíndice.

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




### setArgbColor(int value) {#setArgbColor-int-}
```
public void setArgbColor(int value)
```


Establece el color con un valor ARGB de 32 bits.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Establece un valor que indica si la fuente está en negrita.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCapsType(int value) {#setCapsType-int-}
```
public void setCapsType(int value)
```


Establece el tipo de mayúsculas del texto.

Ver [TextCapsType](../../com.aspose.cells/textcapstype).

**Remarks**

Solo para las fuentes de Shapes o Charts. NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--). Esta propiedad será eliminada 12 meses después, a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCharset(int value) {#setCharset-int-}
```
public void setCharset(int value)
```


Representa el conjunto de caracteres.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Establece el [Color](../../com.aspose.cells/color) de la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDoubleSize(double value) {#setDoubleSize-double-}
```
public void setDoubleSize(double value)
```


Establece el doble tamaño de la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Establece un valor que indica si la fuente está en cursiva.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Establece el nombre de la [Font](../../com.aspose.cells/font).

**Remarks**

Si esta propiedad se usa para establecer el nombre de la fuente, el [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) se actualizará a [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setName(String name, int type) {#setName-java.lang.String-int-}
```
public void setName(String name, int type)
```


Establece el nombre y el esquema de la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String |  |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). |

### setNormalizeHeights(boolean value) {#setNormalizeHeights-boolean-}
```
public void setNormalizeHeights(boolean value)
```


Indica si la normalización de altura debe aplicarse a la ejecución de texto.

**Remarks**

Solo para las fuentes de Shapes o Charts. NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--). Esta propiedad será eliminada 12 meses después, a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSchemeType(int value) {#setSchemeType-int-}
```
public void setSchemeType(int value)
```


Establece el tipo de esquema de la fuente.

Ver [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setScriptOffset(double value) {#setScriptOffset-double-}
```
public void setScriptOffset(double value)
```


Establece el desplazamiento del script, en unidades de porcentaje.

**Remarks**

Solo para formas y gráficos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setSize(int value) {#setSize-int-}
```
public void setSize(int value)
```


Establece el tamaño de la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setStrikeType(int value) {#setStrikeType-int-}
```
public void setStrikeType(int value)
```


Obtiene el tipo de tachado del texto.

Ver [TextStrikeType](../../com.aspose.cells/textstriketype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setStrikeout(boolean value) {#setStrikeout-boolean-}
```
public void setStrikeout(boolean value)
```


Establece un valor que indica si la fuente tiene un tachado simple.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSubscript(boolean value) {#setSubscript-boolean-}
```
public void setSubscript(boolean value)
```


Establece un valor que indica si la fuente está en subíndice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSuperscript(boolean value) {#setSuperscript-boolean-}
```
public void setSuperscript(boolean value)
```


Establece un valor que indica si la fuente está en superíndice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Establece el color del tema.

**Remarks**

Si el color de la fuente no es un color de tema, se devolverá NULL.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setUnderline(int value) {#setUnderline-int-}
```
public void setUnderline(int value)
```


Establece el tipo de subrayado de la fuente.

Ver [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### toString() {#toString--}
```
public String toString()
```


Devuelve una cadena que representa el objeto Cell actual.

**Returns:**
java.lang.String -
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

