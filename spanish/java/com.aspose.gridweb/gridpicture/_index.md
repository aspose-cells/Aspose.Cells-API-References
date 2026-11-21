---
title: "GridPicture"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa una sola imagen en una hoja de cálculo."
type: docs
url: /es/java/com.aspose.gridweb/gridpicture/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridPicture implements IGridSave
```

Encapsula el objeto que representa una sola imagen en una hoja de cálculo.
## Métodos

| Método | Descripción |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Agrega un hipervínculo a la forma. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Mueve la imagen a la esquina superior derecha. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Devuelve o establece la cadena de texto descriptiva (alternativa) del objeto [GridShape](../../com.aspose.gridweb/gridshape). |
| [getBorderLineColor()](#getBorderLineColor--) | Representa el [Color](../../com.aspose.cells/color) de la línea del borde de una imagen. |
| [getBorderWeight()](#getBorderWeight--) | Obtiene el grosor de la línea del borde de una imagen en unidades de pt. |
| [getBottom()](#getBottom--) | Representa el ancho del desplazamiento vertical de la forma desde la fila de su esquina inferior, en unidades de píxeles. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Obtiene los datos de la imagen. |
| [getHeight()](#getHeight--) | Representa la altura de la forma, en unidades de píxel. |
| [getHeightCM()](#getHeightCM--) | Representa la altura de la forma, en unidades de pulgadas. |
| [getHeightInch()](#getHeightInch--) | Representa la altura de la forma, en unidades de pulgadas. |
| [getHeightPt()](#getHeightPt--) | Representa la altura de la forma, en unidades de puntos. |
| [getHeightScale()](#getHeightScale--) | Obtiene la escala de altura, en unidades de porcentaje de la altura original de la imagen. |
| [getHtmlText()](#getHtmlText--) | Obtiene la cadena html que contiene datos y algunos formatos en este cuadro de texto. |
| [getHyperlink()](#getHyperlink--) | Obtiene el hipervínculo de la forma. |
| [getID()](#getID--) | Obtiene /Establece el ID de la imagen. |
| [getImageFormat()](#getImageFormat--) | Obtiene el formato de imagen de la imagen. |
| [getLeft()](#getLeft--) | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxeles. |
| [getLeftCM()](#getLeftCM--) | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de centímetros. |
| [getLeftInch()](#getLeftInch--) | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de pulgadas. |
| [getLeftToCorner()](#getLeftToCorner--) | Representa el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo, en unidades de píxeles. |
| [getLinkedCell()](#getLinkedCell--) | Obtiene el rango de la hoja de cálculo vinculado al valor del control. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Obtiene el desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Obtiene el desplazamiento vertical de la forma desde la fila de su esquina inferior derecha. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Representa el índice de columna de la esquina inferior derecha. |
| [getLowerRightRow()](#getLowerRightRow--) | Representa el índice de fila de la esquina inferior derecha. |
| [getName()](#getName--) | Obtiene el nombre de la forma. |
| [getOriginalHeight()](#getOriginalHeight--) | Obtiene la altura original de la imagen. |
| [getOriginalHeightCM()](#getOriginalHeightCM--) | Obtiene la altura original de la imagen, en unidades de centímetros. |
| [getOriginalHeightInch()](#getOriginalHeightInch--) | Obtiene la altura original de la imagen, en unidades de pulgadas. |
| [getOriginalWidth()](#getOriginalWidth--) | Obtiene el ancho original de la imagen. |
| [getOriginalWidthCM()](#getOriginalWidthCM--) | Obtiene el ancho original de la imagen, en unidades de centímetros. |
| [getOriginalWidthInch()](#getOriginalWidthInch--) | Obtiene el ancho original de la imagen, en unidades de pulgadas. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Indica si la forma es relativa al tamaño original de la imagen. |
| [getRight()](#getRight--) | Representa el ancho del desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha, en unidades de píxeles. |
| [getRotationAngle()](#getRotationAngle--) | Obtiene la rotación de la forma. |
| [getSourceFullName()](#getSourceFullName--) | Obtiene la ruta y el nombre del archivo fuente para la imagen vinculada. |
| [getText()](#getText--) | Representa la cadena en este objeto TextBox. |
| [getTitle()](#getTitle--) | Especifica el título (leyenda) del objeto de forma actual. |
| [getTop()](#getTop--) | Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de píxeles. |
| [getTopCM()](#getTopCM--) | Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de centímetros. |
| [getTopInch()](#getTopInch--) | Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de pulgadas. |
| [getTopToCorner()](#getTopToCorner--) | Representa el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Obtiene el desplazamiento horizontal de la forma desde la columna de su esquina superior izquierda. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Obtiene el desplazamiento vertical de la forma desde la fila de su esquina superior izquierda. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Representa el índice de columna de la esquina superior izquierda. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Representa el índice de fila de la esquina superior izquierda. |
| [getWidth()](#getWidth--) | Representa el ancho de la forma, en unidades de píxeles. |
| [getWidthCM()](#getWidthCM--) | Representa el ancho de la forma, en unidades de centímetros. |
| [getWidthInch()](#getWidthInch--) | Representa el ancho de la forma, en unidades de pulgada. |
| [getWidthPt()](#getWidthPt--) | Representa el ancho de la forma, en unidades de punto. |
| [getWidthScale()](#getWidthScale--) | Obtiene la escala de ancho, en unidades de porcentaje del ancho original de la imagen. |
| [getX()](#getX--) | Obtiene el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo, en unidades de píxeles. |
| [getY()](#getY--) | Obtiene el desplazamiento vertical de la forma desde el borde superior de la hoja, en unidades de píxeles. |
| [getZOrderPosition()](#getZOrderPosition--) | Devuelve la posición de una forma en el orden Z. |
| [hasLine()](#hasLine--) | Obtiene si el borde de línea de la forma es visible. |
| [hashCode()](#hashCode--) |  |
| [isFlippedVertically()](#isFlippedVertically--) | Obtiene si la forma está volteada verticalmente . |
| [isGroup()](#isGroup--) | Indica si la forma es un grupo. |
| [isHidden()](#isHidden--) | Indica si el objeto es visible. |
| [isLockAspectRatio()](#isLockAspectRatio--) | True significa que no se permiten cambios en la relación de aspecto. |
| [isLocked()](#isLocked--) | True si el objeto está bloqueado, False si el objeto puede modificarse cuando la hoja está protegida. |
| [isTextWrapped()](#isTextWrapped--) | Obtiene el tipo de ajuste de texto de la forma que contiene texto. |
| [move(int upperLeftRow, int upperLeftColumn)](#move-int-int-) | Mueve la imagen a una ubicación especificada. |
| [moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)](#moveToRange-int-int-int-int-) | Mueve la forma a un rango especificado. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeHyperlink()](#removeHyperlink--) | Eliminar el hipervínculo de la forma. |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Crea la imagen y la guarda en un flujo. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Devuelve o establece la cadena de texto descriptiva (alternativa) del objeto [GridShape](../../com.aspose.gridweb/gridshape). |
| [setBorderLineColor(Color value)](#setBorderLineColor-com.aspose.gridweb.Color-) | Representa el [Color](../../com.aspose.cells/color) de la línea del borde de una imagen. |
| [setBorderWeight(double value)](#setBorderWeight-double-) | Establece el grosor de la línea del borde de una imagen en unidades de pt. |
| [setBottom(int value)](#setBottom-int-) | Representa el ancho del desplazamiento vertical de la forma desde la fila de su esquina inferior, en unidades de píxeles. |
| [setData(byte[] value)](#setData-byte---) | Obtiene los datos de la imagen. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Establece si la forma está volteada verticalmente. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Establece que el borde de línea de la forma sea visible. |
| [setHeight(int value)](#setHeight-int-) | Representa la altura de la forma, en unidades de píxel. |
| [setHeightCM(double value)](#setHeightCM-double-) | Representa la altura de la forma, en unidades de pulgadas. |
| [setHeightInch(double value)](#setHeightInch-double-) | Representa la altura de la forma, en unidades de pulgadas. |
| [setHeightPt(double value)](#setHeightPt-double-) | Representa la altura de la forma, en unidades de puntos. |
| [setHeightScale(int value)](#setHeightScale-int-) | Establece la escala de altura, en unidades de porcentaje de la altura original de la imagen. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indica si el objeto es visible. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Establece la cadena html que contiene datos y algunos formatos en este cuadro de texto. |
| [setID(String value)](#setID-java.lang.String-) | Obtiene /Establece el ID de la imagen. |
| [setLeft(int value)](#setLeft-int-) | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxeles. |
| [setLeftCM(double value)](#setLeftCM-double-) | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de centímetros. |
| [setLeftInch(double value)](#setLeftInch-double-) | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de pulgadas. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Representa el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo, en unidades de píxeles. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Establece el rango de la hoja de cálculo vinculado al valor del control. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | True significa que no se permiten cambios en la relación de aspecto. |
| [setLocked(boolean value)](#setLocked-boolean-) | True si el objeto está bloqueado, False si el objeto puede modificarse cuando la hoja está protegida. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Establece el desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Establece el desplazamiento vertical de la forma desde la fila de su esquina inferior derecha. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Representa el índice de columna de la esquina inferior derecha. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Representa el índice de fila de la esquina inferior derecha. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre de la forma. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Indica si la forma es relativa al tamaño original de la imagen. |
| [setRight(int value)](#setRight-int-) | Representa el ancho del desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha, en unidades de píxeles. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Establece la rotación de la forma. |
| [setSourceFullName(String value)](#setSourceFullName-java.lang.String-) | Establece la ruta y el nombre del archivo fuente para la imagen vinculada. |
| [setText(String value)](#setText-java.lang.String-) | Representa la cadena en este objeto TextBox. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Establece el tipo de ajuste de texto de la forma que contiene texto. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Especifica el título (leyenda) del objeto de forma actual. |
| [setTop(int value)](#setTop-int-) | Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de píxeles. |
| [setTopCM(double value)](#setTopCM-double-) | Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de centímetros. |
| [setTopInch(double value)](#setTopInch-double-) | Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de pulgadas. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Representa el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Establece el desplazamiento horizontal de la forma desde la columna de su esquina superior izquierda. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Establece el desplazamiento vertical de la forma desde la fila de su esquina superior izquierda. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Representa el índice de columna de la esquina superior izquierda. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Representa el índice de fila de la esquina superior izquierda. |
| [setWidth(int value)](#setWidth-int-) | Representa el ancho de la forma, en unidades de píxeles. |
| [setWidthCM(double value)](#setWidthCM-double-) | Representa el ancho de la forma, en unidades de centímetros. |
| [setWidthInch(double value)](#setWidthInch-double-) | Representa el ancho de la forma, en unidades de pulgada. |
| [setWidthPt(double value)](#setWidthPt-double-) | Representa el ancho de la forma, en unidades de punto. |
| [setWidthScale(int value)](#setWidthScale-int-) | Establece la escala de ancho, en unidades de porcentaje del ancho original de la imagen. |
| [setX(int value)](#setX-int-) | Establece el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja, en unidades de píxeles. |
| [setY(int value)](#setY-int-) | Establece el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Devuelve la posición de una forma en el orden Z. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public GridHyperlink addHyperlink(String address)
```


Agrega un hipervínculo a la forma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dirección | java.lang.String | Dirección del hipervínculo. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - Return the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Mueve la imagen a la esquina superior derecha.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | el índice de fila. |
| rightColumn | int | el índice de la columna. |

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Devuelve o establece la cadena de texto descriptiva (alternativa) del objeto [GridShape](../../com.aspose.gridweb/gridshape).

**Returns:**
java.lang.String
### getBorderLineColor() {#getBorderLineColor--}
```
public Color getBorderLineColor()
```


Representa el [Color](../../com.aspose.cells/color) de la línea del borde de una imagen.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderWeight() {#getBorderWeight--}
```
public double getBorderWeight()
```


Obtiene el grosor de la línea del borde de una imagen en unidades de pt.

**Returns:**
double
### getBottom() {#getBottom--}
```
public int getBottom()
```


Representa el ancho del desplazamiento vertical de la forma desde la fila de su esquina inferior, en unidades de píxeles.

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


Obtiene los datos de la imagen.

**Returns:**
byte[]
### getHeight() {#getHeight--}
```
public int getHeight()
```


Representa la altura de la forma, en unidades de píxel.

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


Representa la altura de la forma, en unidades de pulgadas.

**Returns:**
double
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


Representa la altura de la forma, en unidades de pulgadas.

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


Representa la altura de la forma, en unidades de puntos.

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


Obtiene la escala de altura, en unidades de porcentaje de la altura original de la imagen. Si la forma no es una imagen, la propiedad HeightScale solo devuelve 100;

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


Obtiene la cadena html que contiene datos y algunos formatos en este cuadro de texto.

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public GridHyperlink getHyperlink()
```


Obtiene el hipervínculo de la forma.

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink)
### getID() {#getID--}
```
public String getID()
```


Obtiene /Establece el ID de la imagen.

**Returns:**
java.lang.String
### getImageFormat() {#getImageFormat--}
```
public int getImageFormat()
```


Obtiene el formato de imagen de la imagen.

Ver [GridImageType](../../com.aspose.gridweb/gridimagetype).

**Returns:**
int
### getLeft() {#getLeft--}
```
public int getLeft()
```


Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxeles.

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de centímetros.

**Returns:**
double
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de pulgadas.

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Representa el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo, en unidades de píxeles.

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Obtiene el rango de la hoja de cálculo vinculado al valor del control.

**Returns:**
java.lang.String
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


Obtiene el desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha. El rango de valores es de 0 a 1024.

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


Obtiene el desplazamiento vertical de la forma desde la fila de su esquina inferior derecha. El rango de valores es de 0 a 256.

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


Representa el índice de columna de la esquina inferior derecha.

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


Representa el índice de fila de la esquina inferior derecha.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre de la forma.

**Returns:**
java.lang.String
### getOriginalHeight() {#getOriginalHeight--}
```
public int getOriginalHeight()
```


Obtiene la altura original de la imagen.

**Returns:**
int
### getOriginalHeightCM() {#getOriginalHeightCM--}
```
public double getOriginalHeightCM()
```


Obtiene la altura original de la imagen, en unidades de centímetros.

**Returns:**
double
### getOriginalHeightInch() {#getOriginalHeightInch--}
```
public double getOriginalHeightInch()
```


Obtiene la altura original de la imagen, en unidades de pulgadas.

**Returns:**
double
### getOriginalWidth() {#getOriginalWidth--}
```
public int getOriginalWidth()
```


Obtiene el ancho original de la imagen.

**Returns:**
int
### getOriginalWidthCM() {#getOriginalWidthCM--}
```
public double getOriginalWidthCM()
```


Obtiene el ancho original de la imagen, en unidades de centímetros.

**Returns:**
double
### getOriginalWidthInch() {#getOriginalWidthInch--}
```
public double getOriginalWidthInch()
```


Obtiene el ancho original de la imagen, en unidades de pulgadas.

**Returns:**
double
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


Indica si la forma es relativa al tamaño original de la imagen.

**Returns:**
boolean
### getRight() {#getRight--}
```
public int getRight()
```


Representa el ancho del desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha, en unidades de píxeles.

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


Obtiene la rotación de la forma.

**Returns:**
double
### getSourceFullName() {#getSourceFullName--}
```
public String getSourceFullName()
```


Obtiene la ruta y el nombre del archivo fuente para la imagen vinculada.

**Remarks**

El valor predeterminado es una cadena vacía. Si SourceFullName no es una cadena vacía, la imagen está vinculada. Si SourceFullName no es una cadena vacía, pero Data es nulo, entonces la imagen está vinculada y no se almacena en el archivo.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Representa la cadena en este objeto TextBox.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Especifica el título (leyenda) del objeto de forma actual.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de píxeles.

**Remarks**

Si la forma está en el gráfico, representa el desplazamiento vertical de la forma desde su borde superior.

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de centímetros.

**Returns:**
double
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de pulgadas.

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Representa el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles.

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


Obtiene el desplazamiento horizontal de la forma desde la columna de su esquina superior izquierda. El rango de valores es de 0 a 1024.

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


Obtiene el desplazamiento vertical de la forma desde la fila de su esquina superior izquierda. El rango de valores es de 0 a 256.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Representa el índice de columna de la esquina superior izquierda.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Representa el índice de fila de la esquina superior izquierda.

**Remarks**

Si la forma está dentro de otra forma o en el grupo, UpperLeftRow será ignorado.

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Representa el ancho de la forma, en unidades de píxeles.

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


Representa el ancho de la forma, en unidades de centímetros.

**Returns:**
double
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


Representa el ancho de la forma, en unidades de pulgada.

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


Representa el ancho de la forma, en unidades de punto.

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


Obtiene la escala de ancho, en unidades de porcentaje del ancho original de la imagen. Si la forma no es una imagen, la propiedad WidthScale solo devuelve 100;

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


Obtiene el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo, en unidades de píxeles.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Obtiene el desplazamiento vertical de la forma desde el borde superior de la hoja, en unidades de píxeles.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Devuelve la posición de una forma en el orden Z.

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


Obtiene si el borde de línea de la forma es visible.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFlippedVertically() {#isFlippedVertically--}
```
public boolean isFlippedVertically()
```


Obtiene si la forma está volteada verticalmente .

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


Indica si la forma es un grupo.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indica si el objeto es visible.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


True significa que no se permiten cambios en la relación de aspecto.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


True si el objeto está bloqueado, False si el objeto puede modificarse cuando la hoja está protegida.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Obtiene el tipo de ajuste de texto de la forma que contiene texto.

**Returns:**
boolean
### move(int upperLeftRow, int upperLeftColumn) {#move-int-int-}
```
public void move(int upperLeftRow, int upperLeftColumn)
```


Mueve la imagen a una ubicación especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| upperLeftRow | int | Índice de fila superior izquierda. |
| upperLeftColumn | int | Índice de columna superior izquierda. |

### moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)
```


Mueve la forma a un rango especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| upperLeftRow | int | Índice de fila superior izquierda. |
| upperLeftColumn | int | Índice de columna superior izquierda. |
| lowerRightRow | int | Índice de fila inferior derecha |
| lowerRightColumn | int | Índice de columna inferior derecha |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeHyperlink() {#removeHyperlink--}
```
public void removeHyperlink()
```


Eliminar el hipervínculo de la forma.

### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


Crea la imagen y la guarda en un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Devuelve o establece la cadena de texto descriptiva (alternativa) del objeto [GridShape](../../com.aspose.gridweb/gridshape).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setBorderLineColor(Color value) {#setBorderLineColor-com.aspose.gridweb.Color-}
```
public void setBorderLineColor(Color value)
```


Representa el [Color](../../com.aspose.cells/color) de la línea del borde de una imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderWeight(double value) {#setBorderWeight-double-}
```
public void setBorderWeight(double value)
```


Establece el grosor de la línea del borde de una imagen en unidades de pt.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


Representa el ancho del desplazamiento vertical de la forma desde la fila de su esquina inferior, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setData(byte[] value) {#setData-byte---}
```
public void setData(byte[] value)
```


Obtiene los datos de la imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte[] |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


Establece si la forma está volteada verticalmente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasLine(boolean value) {#setHasLine-boolean-}
```
public void setHasLine(boolean value)
```


Establece que el borde de línea de la forma sea visible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Representa la altura de la forma, en unidades de píxel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


Representa la altura de la forma, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


Representa la altura de la forma, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setHeightPt(double value) {#setHeightPt-double-}
```
public void setHeightPt(double value)
```


Representa la altura de la forma, en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setHeightScale(int value) {#setHeightScale-int-}
```
public void setHeightScale(int value)
```


Establece la escala de altura, en unidades de porcentaje de la altura original de la imagen. Si la forma no es una imagen, la propiedad HeightScale solo devuelve 100;

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indica si el objeto es visible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHtmlText(String value) {#setHtmlText-java.lang.String-}
```
public void setHtmlText(String value)
```


Establece la cadena html que contiene datos y algunos formatos en este cuadro de texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


Obtiene /Establece el ID de la imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setLeft(int value) {#setLeft-int-}
```
public void setLeft(int value)
```


Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLeftCM(double value) {#setLeftCM-double-}
```
public void setLeftCM(double value)
```


Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de centímetros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setLeftInch(double value) {#setLeftInch-double-}
```
public void setLeftInch(double value)
```


Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


Representa el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Establece el rango de la hoja de cálculo vinculado al valor del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


True significa que no se permiten cambios en la relación de aspecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


True si el objeto está bloqueado, False si el objeto puede modificarse cuando la hoja está protegida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


Establece el desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha. El rango de valores es de 0 a 1024.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


Establece el desplazamiento vertical de la forma desde la fila de su esquina inferior derecha. El rango de valores es de 0 a 256.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLowerRightColumn(int value) {#setLowerRightColumn-int-}
```
public void setLowerRightColumn(int value)
```


Representa el índice de columna de la esquina inferior derecha.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLowerRightRow(int value) {#setLowerRightRow-int-}
```
public void setLowerRightRow(int value)
```


Representa el índice de fila de la esquina inferior derecha.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Establece el nombre de la forma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setRelativeToOriginalPictureSize(boolean value) {#setRelativeToOriginalPictureSize-boolean-}
```
public void setRelativeToOriginalPictureSize(boolean value)
```


Indica si la forma es relativa al tamaño original de la imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRight(int value) {#setRight-int-}
```
public void setRight(int value)
```


Representa el ancho del desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Establece la rotación de la forma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setSourceFullName(String value) {#setSourceFullName-java.lang.String-}
```
public void setSourceFullName(String value)
```


Establece la ruta y el nombre del archivo fuente para la imagen vinculada.

**Remarks**

El valor predeterminado es una cadena vacía. Si SourceFullName no es una cadena vacía, la imagen está vinculada. Si SourceFullName no es una cadena vacía, pero Data es nulo, entonces la imagen está vinculada y no se almacena en el archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Representa la cadena en este objeto TextBox.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Establece el tipo de ajuste de texto de la forma que contiene texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Especifica el título (leyenda) del objeto de forma actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTop(int value) {#setTop-int-}
```
public void setTop(int value)
```


Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de píxeles.

**Remarks**

Si la forma está en el gráfico, representa el desplazamiento vertical de la forma desde su borde superior.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTopCM(double value) {#setTopCM-double-}
```
public void setTopCM(double value)
```


Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de centímetros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setTopInch(double value) {#setTopInch-double-}
```
public void setTopInch(double value)
```


Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


Representa el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


Establece el desplazamiento horizontal de la forma desde la columna de su esquina superior izquierda. El rango de valores es de 0 a 1024.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


Establece el desplazamiento vertical de la forma desde la fila de su esquina superior izquierda. El rango de valores es de 0 a 256.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setUpperLeftColumn(int value) {#setUpperLeftColumn-int-}
```
public void setUpperLeftColumn(int value)
```


Representa el índice de columna de la esquina superior izquierda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setUpperLeftRow(int value) {#setUpperLeftRow-int-}
```
public void setUpperLeftRow(int value)
```


Representa el índice de fila de la esquina superior izquierda.

**Remarks**

Si la forma está dentro de otra forma o en el grupo, UpperLeftRow será ignorado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Representa el ancho de la forma, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


Representa el ancho de la forma, en unidades de centímetros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


Representa el ancho de la forma, en unidades de pulgada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWidthPt(double value) {#setWidthPt-double-}
```
public void setWidthPt(double value)
```


Representa el ancho de la forma, en unidades de punto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWidthScale(int value) {#setWidthScale-int-}
```
public void setWidthScale(int value)
```


Establece la escala de ancho, en unidades de porcentaje del ancho original de la imagen. Si la forma no es una imagen, la propiedad WidthScale solo devuelve 100;

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Establece el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Establece el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


Devuelve la posición de una forma en el orden Z.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

