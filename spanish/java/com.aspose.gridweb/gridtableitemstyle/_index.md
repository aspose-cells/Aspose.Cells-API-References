---
title: "GridTableItemStyle"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Hereda de System.Web.UI.WebControls.TableItemStyle."
type: docs
url: /es/java/com.aspose.gridweb/gridtableitemstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebStyle](../../com.aspose.gridweb/webstyle), [com.aspose.gridweb.WebTableItemStyle](../../com.aspose.gridweb/webtableitemstyle)
```
public class GridTableItemStyle extends WebTableItemStyle
```

Heredado de System.Web.UI.WebControls.TableItemStyle. Encapsula los estilos de un WebCell.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheetCollection sheets = GridWeb1.getWorkSheets();
 
         GridWorksheet sheet = sheets.add("demo1");
 
         sheet.getCells().get(0,0).putValue("Demo Text");
         GridTableItemStyle style = sheet.getCells().get(0, 0).getStyle();
 
         style.getFont().setSize(FontUnit.Point(72));
         style.setWrap(false);
 
         style.setBackColor(Color.getGray());
         	style.setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         style.setBorderWidth(Unit.Pixel(1));
         style.setBorderColor(Color.getSilver());
         style.getRightBorderStyle().setBorderColor(Color.getBlack());
         	style.getRightBorderStyle().setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         	style.getRightBorderStyle().setBorderWidth(Unit.Pixel(1));
         style.getBottomBorderStyle().setBorderColor(Color.getBlack());
         style.getBottomBorderStyle().setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         style.getBottomBorderStyle().setBorderWidth(Unit.Pixel(1));
         sheet.getCells().get(0, 0).setStyle(style);
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GridTableItemStyle()](#GridTableItemStyle--) | Constructor predeterminado. |
## Métodos

| Método | Descripción |
| --- | --- |
| [copyFrom(WebStyle s)](#copyFrom-com.aspose.gridweb.WebStyle-) | Copia de otro objeto de estilo. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | Obtiene el BackColor en el estilo |
| [getBackImageAttributes()](#getBackImageAttributes--) | Atributos de la imagen de fondo. |
| [getBackImageUrl()](#getBackImageUrl--) | URL de la imagen de fondo. |
| [getBorderColor()](#getBorderColor--) | Obtiene el BorderColor en el estilo |
| [getBorderStyle()](#getBorderStyle--) | Obtiene el BorderStyle en el estilo |
| [getBorderWidth()](#getBorderWidth--) | Obtiene el BorderWidth en el estilo |
| [getBottomBorderStyle()](#getBottomBorderStyle--) | Especifica el estilo del borde inferior de la celda. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | Obtiene el CssClass en el estilo |
| [getCustom()](#getCustom--) | Obtiene el formato personalizado; null o cadena vacía significa que no hay formato personalizado. |
| [getFont()](#getFont--) | Obtiene la Font en el estilo |
| [getForeColor()](#getForeColor--) | Obtiene el ForeColor en el estilo |
| [getHeight()](#getHeight--) | Obtiene la Height en el estilo |
| [getHorizontalAlign()](#getHorizontalAlign--) | Obtiene el HorizontalAlign en el estilo |
| [getIndentLevel()](#getIndentLevel--) | Obtiene el nivel de sangría. |
| [getLeftBorderStyle()](#getLeftBorderStyle--) | Especifica el estilo del borde izquierdo de la celda. |
| [getNumberType()](#getNumberType--) | Obtiene el formato de visualización de números y fechas. |
| [getQuotePrefix()](#getQuotePrefix--) | Indica si el valor de la celda comienza con una comilla simple. |
| [getRightBorderStyle()](#getRightBorderStyle--) | Especifica el estilo del borde derecho de la celda. |
| [getRotationAngle()](#getRotationAngle--) | Obtiene el atributo Rotación. |
| [getTopBorderStyle()](#getTopBorderStyle--) | Especifica el estilo del borde superior de la celda. |
| [getVerticalAlign()](#getVerticalAlign--) | Obtiene la alineación vertical en el estilo. |
| [getWidth()](#getWidth--) | Obtiene el Width en el estilo |
| [getWrap()](#getWrap--) | Obtiene el ajuste de texto en el estilo. |
| [hashCode()](#hashCode--) | Sirve como función hash para un tipo particular, adecuada para su uso en algoritmos de hash y estructuras de datos como una tabla hash. |
| [isLocked()](#isLocked--) | Obtiene un valor que indica si una celda puede modificarse o no cuando su hoja de cálculo está protegida. |
| [mergeWith(WebStyle s)](#mergeWith-com.aspose.gridweb.WebStyle-) | Fusiona con otro objeto de estilo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | Establece el BackColor en el estilo |
| [setBackImageAttributes(String value)](#setBackImageAttributes-java.lang.String-) | Atributos de la imagen de fondo. |
| [setBackImageUrl(String value)](#setBackImageUrl-java.lang.String-) | URL de la imagen de fondo. |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | Establece el BorderColor en el estilo |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Establece el BorderStyle en el estilo |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | Establece el BorderWidth en el estilo |
| [setBottomBorderStyle(WebBorderStyle value)](#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Especifica el estilo del borde inferior de la celda. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | Establece el CssClass en el estilo |
| [setCustom(String value)](#setCustom-java.lang.String-) | Establece el formato personalizado; null o cadena vacía significa que no hay formato personalizado. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | Establece el ForeColor en el estilo |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Establece el Height en el estilo |
| [setHorizontalAlign(int value)](#setHorizontalAlign-int-) | Establece el HorizontalAlign en el estilo |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Establece el nivel de sangría. |
| [setLeftBorderStyle(WebBorderStyle value)](#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Especifica el estilo del borde izquierdo de la celda. |
| [setLocked(boolean value)](#setLocked-boolean-) | Establece un valor que indica si una celda puede modificarse o no cuando su hoja de cálculo está protegida. |
| [setNumberType(int value)](#setNumberType-int-) | Establece el formato de visualización de números y fechas. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Indica si el valor de la celda comienza con una comilla simple. |
| [setRightBorderStyle(WebBorderStyle value)](#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Especifica el estilo del borde derecho de la celda. |
| [setRotationAngle(short value)](#setRotationAngle-short-) | Establece el atributo Rotación. |
| [setTopBorderStyle(WebBorderStyle value)](#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Especifica el estilo del borde superior de la celda. |
| [setVerticalAlign(int value)](#setVerticalAlign-int-) | Establece la alineación vertical en el estilo. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Establece el Width en el estilo |
| [setWrap(boolean value)](#setWrap-boolean-) | Establece el ajuste de texto en el estilo. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTableItemStyle() {#GridTableItemStyle--}
```
public GridTableItemStyle()
```


Constructor predeterminado.

### copyFrom(WebStyle s) {#copyFrom-com.aspose.gridweb.WebStyle-}
```
public void copyFrom(WebStyle s)
```


Copia de otro objeto de estilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | otro objeto de estilo |

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
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Obtiene el BackColor en el estilo

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBackImageAttributes() {#getBackImageAttributes--}
```
public String getBackImageAttributes()
```


Atributos de la imagen de fondo.

**Returns:**
java.lang.String
### getBackImageUrl() {#getBackImageUrl--}
```
public String getBackImageUrl()
```


URL de la imagen de fondo.

**Returns:**
java.lang.String
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


Obtiene el BorderColor en el estilo

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Obtiene el BorderStyle en el estilo

Ver [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


Obtiene el BorderWidth en el estilo

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomBorderStyle() {#getBottomBorderStyle--}
```
public WebBorderStyle getBottomBorderStyle()
```


Especifica el estilo del borde inferior de la celda.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssClass() {#getCssClass--}
```
public String getCssClass()
```


Obtiene el CssClass en el estilo

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


Obtiene el formato personalizado; null o cadena vacía significa que no hay formato personalizado.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public FontInfo getFont()
```


Obtiene la Font en el estilo

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Obtiene el ForeColor en el estilo

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```


Obtiene la Height en el estilo

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHorizontalAlign() {#getHorizontalAlign--}
```
public int getHorizontalAlign()
```


Obtiene el HorizontalAlign en el estilo

Ver [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


Obtiene el nivel de sangría.

**Remarks**

**Returns:**
int
### getLeftBorderStyle() {#getLeftBorderStyle--}
```
public WebBorderStyle getLeftBorderStyle()
```


Especifica el estilo del borde izquierdo de la celda.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```


Obtiene el formato de visualización de números y fechas. Los patrones de formato son diferentes para distintas regiones.

**Remarks**

Por ejemplo, los patrones de formato representados por números para la región en\_US:

| Value | Tipo | Cadena de formato |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Red](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm AM/PM` |
| 19 | Time | `h:mm:ss AM/PM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Red](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Red](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```


Indica si el valor de la celda comienza con una comilla simple.

**Returns:**
boolean
### getRightBorderStyle() {#getRightBorderStyle--}
```
public WebBorderStyle getRightBorderStyle()
```


Especifica el estilo del borde derecho de la celda.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getRotationAngle() {#getRotationAngle--}
```
public short getRotationAngle()
```


Obtiene el atributo Rotación.

**Remarks**

0: No rotado.

255: De arriba a abajo.

\-90: Hacia abajo.

90: Hacia arriba.

Puede establecer 255 o un valor en el rango de -90 a 90.

**Returns:**
short
### getTopBorderStyle() {#getTopBorderStyle--}
```
public WebBorderStyle getTopBorderStyle()
```


Especifica el estilo del borde superior de la celda.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getVerticalAlign() {#getVerticalAlign--}
```
public int getVerticalAlign()
```


Obtiene la alineación vertical en el estilo.

Ver [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Returns:**
int
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Obtiene el Width en el estilo

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWrap() {#getWrap--}
```
public boolean getWrap()
```


Obtiene el ajuste de texto en el estilo.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Sirve como función hash para un tipo particular, adecuada para su uso en algoritmos de hash y estructuras de datos como una tabla hash.

**Returns:**
int - Un código hash para el estilo actual.
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Obtiene un valor que indica si una celda puede modificarse o no cuando su hoja de cálculo está protegida. Cuando la hoja está protegida y IsLocked es verdadero, la celda no puede editarse. Cuando la hoja está protegida y IsLocked es falso, la celda puede editarse.

**Returns:**
boolean
### mergeWith(WebStyle s) {#mergeWith-com.aspose.gridweb.WebStyle-}
```
public void mergeWith(WebStyle s)
```


Fusiona con otro objeto de estilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | otro objeto de estilo |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```


Establece el BackColor en el estilo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBackImageAttributes(String value) {#setBackImageAttributes-java.lang.String-}
```
public void setBackImageAttributes(String value)
```


Atributos de la imagen de fondo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setBackImageUrl(String value) {#setBackImageUrl-java.lang.String-}
```
public void setBackImageUrl(String value)
```


URL de la imagen de fondo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


Establece el BorderColor en el estilo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Establece el BorderStyle en el estilo

Ver [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


Establece el BorderWidth en el estilo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomBorderStyle(WebBorderStyle value) {#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setBottomBorderStyle(WebBorderStyle value)
```


Especifica el estilo del borde inferior de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


Establece el CssClass en el estilo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


Establece el formato personalizado; null o cadena vacía significa que no hay formato personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


Establece el ForeColor en el estilo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


Establece el Height en el estilo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHorizontalAlign(int value) {#setHorizontalAlign-int-}
```
public void setHorizontalAlign(int value)
```


Establece el HorizontalAlign en el estilo

Ver [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


Establece el nivel de sangría.

**Remarks**

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLeftBorderStyle(WebBorderStyle value) {#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setLeftBorderStyle(WebBorderStyle value)
```


Especifica el estilo del borde izquierdo de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Establece un valor que indica si una celda puede modificarse o no cuando su hoja de cálculo está protegida. Cuando la hoja está protegida y IsLocked es verdadero, la celda no puede editarse. Cuando la hoja está protegida y IsLocked es falso, la celda puede editarse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


Establece el formato de visualización de números y fechas. Los patrones de formato son diferentes para distintas regiones.

**Remarks**

Por ejemplo, los patrones de formato representados por números para la región en\_US:

| Value | Tipo | Cadena de formato |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Red](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm AM/PM` |
| 19 | Time | `h:mm:ss AM/PM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Red](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Red](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


Indica si el valor de la celda comienza con una comilla simple.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRightBorderStyle(WebBorderStyle value) {#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setRightBorderStyle(WebBorderStyle value)
```


Especifica el estilo del borde derecho de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setRotationAngle(short value) {#setRotationAngle-short-}
```
public void setRotationAngle(short value)
```


Establece el atributo Rotación.

**Remarks**

0: No rotado.

255: De arriba a abajo.

\-90: Hacia abajo.

90: Hacia arriba.

Puede establecer 255 o un valor en el rango de -90 a 90.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | short |  |

### setTopBorderStyle(WebBorderStyle value) {#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setTopBorderStyle(WebBorderStyle value)
```


Especifica el estilo del borde superior de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setVerticalAlign(int value) {#setVerticalAlign-int-}
```
public void setVerticalAlign(int value)
```


Establece la alineación vertical en el estilo.

Ver [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Establece el Width en el estilo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setWrap(boolean value) {#setWrap-boolean-}
```
public void setWrap(boolean value)
```


Establece el ajuste de texto en el estilo.

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

