---
title: "Label"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa una etiqueta en una hoja de cálculo."
type: docs
url: /es/java/com.aspose.cells/label/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Shape](../../com.aspose.cells/shape)
```
public class Label extends Shape
```

Encapsula el objeto que representa una etiqueta en una hoja de cálculo.

**Example**

```
         //Create a new Workbook.
         Workbook workbook = new Workbook();
 
         //Get the first worksheet in the workbook.
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Add a new label to the worksheet.
         Label label = sheet.getShapes().addLabel(2, 0, 2, 0, 60, 120);
 
         //Set the caption of the label.
         label.setText("This is a Label");
 
         //Set the Placement Type, the way the
         //label is attached to the cells.
         label.setPlacement(PlacementType.FREE_FLOATING);
 
         //Set the fill color of the label.
         label.getFill().setFillType(FillType.SOLID);
         label.getFill().getSolidFill().setColor(Color.getYellow());
 
         //Saves the file.
         workbook.save("tstlabel.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Agrega un hipervínculo a la forma. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Mueve la imagen a la esquina superior derecha. |
| [calculateTextSize()](#calculateTextSize--) | Recalcular el área de texto |
| [characters(int startIndex, int length)](#characters-int-int-) | Devuelve un objeto Characters que representa un rango de caracteres dentro del texto. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fitToTextSize()](#fitToTextSize--) | Recalcula un área de texto adecuada para mostrar todo el contenido del texto. |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Da formato a algunos caracteres con la configuración de fuente. |
| [getActiveXControl()](#getActiveXControl--) | Obtiene el control ActiveX. |
| [getActualBox()](#getActualBox--) | Obtenga la posición y el tamaño reales de la forma (después de aplicar rotación, volteo, etc.) |
| [getActualLowerRightRow()](#getActualLowerRightRow--) | Obtenga la fila inferior real. |
| [getAlternativeText()](#getAlternativeText--) | Devuelve o establece la cadena de texto descriptiva (alternativa) del objeto [Shape](../../com.aspose.cells/shape). |
| [getAnchorType()](#getAnchorType--) | Obtiene el tipo del marcador de posición del ancla de la forma. |
| [getAutoShapeType()](#getAutoShapeType--) | Obtiene el tipo de forma automática. |
| [getBottom()](#getBottom--) | Representa el ancho del desplazamiento vertical de la forma desde la fila de su esquina inferior, en unidades de píxeles. |
| [getCharacters()](#getCharacters--) | Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto. |
| [getClass()](#getClass--) |  |
| [getConnectionPoints()](#getConnectionPoints--) | Obtiene los puntos de conexión |
| [getControlData()](#getControlData--) | Obtiene los datos del control. |
| [getCreateId()](#getCreateId--) | Obtiene el id de creación para esta forma. |
| [getFill()](#getFill--) | Devuelve un objeto [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--) que contiene las propiedades de formato de relleno para la forma especificada. |
| [getFillFormat()](#getFillFormat--) | Devuelve un objeto MsoFillFormat que contiene las propiedades de formato de relleno para la forma especificada. |
| [getFont()](#getFont--) | Representa la fuente de la forma. |
| [getFormatPicture()](#getFormatPicture--) | Obtiene las opciones del formato de imagen. |
| [getGeometry()](#getGeometry--) | Obtiene la geometría |
| [getGlow()](#getGlow--) | Representa un objeto [GlowEffect](../../com.aspose.cells/gloweffect) que especifica el efecto de resplandor para el elemento del gráfico o la forma. |
| [getGroup()](#getGroup--) | Obtiene el grupo de formas que contiene esta forma. |
| [getHeight()](#getHeight--) | Representa la altura de la forma, en unidades de píxel. |
| [getHeightCM()](#getHeightCM--) | Representa la altura de la forma, en unidades de centímetros. |
| [getHeightInShape()](#getHeightInShape--) | Representa el desplazamiento vertical de la forma desde el borde superior de la forma padre, en unidades de 1/4000 de la altura de la forma padre. |
| [getHeightInch()](#getHeightInch--) | Representa la altura de la forma, en unidades de pulgadas. |
| [getHeightPt()](#getHeightPt--) | Representa la altura de la forma, en unidades de puntos. |
| [getHeightScale()](#getHeightScale--) | Obtiene la escala de altura, en unidades de porcentaje de la altura original de la imagen. |
| [getHtmlText()](#getHtmlText--) | Obtiene la cadena HTML que contiene datos y algunos formatos en este cuadro de texto. |
| [getHyperlink()](#getHyperlink--) | Obtiene el hipervínculo de la forma. |
| [getId()](#getId--) | Obtiene el identificador de esta forma. |
| [getInputRange()](#getInputRange--) | Obtiene el rango de hoja de cálculo utilizado para rellenar el cuadro combinado especificado. |
| [getInputRange(boolean isR1C1, boolean isLocal)](#getInputRange-boolean-boolean-) | Obtiene el rango utilizado para rellenar el control. |
| [getLeft()](#getLeft--) | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxeles. |
| [getLeftCM()](#getLeftCM--) | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de centímetros. |
| [getLeftInShape()](#getLeftInShape--) | Representa el desplazamiento horizontal de la forma desde el borde izquierdo de la forma padre, en unidades de 1/4000 del ancho de la forma padre. |
| [getLeftInch()](#getLeftInch--) | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de pulgadas. |
| [getLeftToCorner()](#getLeftToCorner--) | Obtiene el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo. |
| [getLine()](#getLine--) | Obtiene el estilo de línea |
| [getLineFormat()](#getLineFormat--) | Devuelve un objeto MsoLineFormat que contiene las propiedades de formato de línea para la forma especificada. |
| [getLinkedCell()](#getLinkedCell--) | Obtiene el rango de la hoja de cálculo vinculado al valor del control. |
| [getLinkedCell(boolean isR1C1, boolean isLocal)](#getLinkedCell-boolean-boolean-) | Obtiene el rango vinculado al valor del control. |
| [getLockedProperty(int type)](#getLockedProperty-int-) | Obtiene el valor de la propiedad locked. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Obtiene el desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Obtiene el desplazamiento vertical de la forma desde la fila de su esquina inferior derecha. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Representa el índice de columna de la esquina inferior derecha. |
| [getLowerRightRow()](#getLowerRightRow--) | Representa el índice de fila de la esquina inferior derecha. |
| [getMacroName()](#getMacroName--) | Obtiene el nombre de la macro. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Obtiene el tipo de dibujo. |
| [getName()](#getName--) | Obtiene el nombre de la forma. |
| [getPaths()](#getPaths--) | Obtiene las rutas de una forma geométrica personalizada. |
| [getPlacement()](#getPlacement--) | Representa la forma en que el objeto de dibujo está unido a las celdas debajo de él. |
| [getReflection()](#getReflection--) | Representa un objeto [ReflectionEffect](../../com.aspose.cells/reflectioneffect) que especifica el efecto de reflexión para el elemento de gráfico o forma. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Indica si la forma es relativa al tamaño original de la imagen. |
| [getResultOfSmartArt()](#getResultOfSmartArt--) | Convirtiendo arte inteligente a formas agrupadas. |
| [getRichFormattings()](#getRichFormattings--) | Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto. |
| [getRight()](#getRight--) | Representa el ancho del desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha, en unidades de píxeles. |
| [getRotationAngle()](#getRotationAngle--) | Obtiene la rotación de la forma. |
| [getShadowEffect()](#getShadowEffect--) | Representa un objeto [ShadowEffect](../../com.aspose.cells/shadoweffect) que especifica el efecto de sombra para el elemento de gráfico o forma. |
| [getSoftEdges()](#getSoftEdges--) | Obtiene el radio del desenfoque que se aplicará a los bordes, en unidades de puntos. |
| [getSpid()](#getSpid--) | Especifica un identificador de cadena opcional que una aplicación puede usar para identificar la forma particular. |
| [getSpt()](#getSpt--) | Especifica un número opcional que una aplicación puede usar para asociar la forma particular con un tipo de forma definido. |
| [getText()](#getText--) | Obtiene el texto de esta forma. |
| [getTextBody()](#getTextBody--) | Obtiene la configuración del texto de la forma. |
| [getTextBoxOptions()](#getTextBoxOptions--) | Obtiene la información de texto en la forma |
| [getTextDirection()](#getTextDirection--) | Obtiene la dirección del flujo de texto para este objeto. |
| [getTextEffect()](#getTextEffect--) | Devuelve un objeto TextEffectFormat que contiene propiedades de formato de efectos de texto para la forma especificada. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Obtiene el tipo de alineación horizontal del texto de la forma. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Obtiene el tipo de desbordamiento horizontal del texto de la forma que contiene texto. |
| [getTextOptions()](#getTextOptions--) | Representa las opciones de texto de la forma. |
| [getTextOrientationType()](#getTextOrientationType--) | Obtiene el tipo de orientación del texto de la forma. |
| [getTextShapeType()](#getTextShapeType--) | Obtiene el tipo de forma de texto predefinido. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Obtiene el tipo de alineación vertical del texto de la forma. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Obtiene el tipo de desbordamiento vertical del texto de la forma que contiene texto. |
| [getThreeDFormat()](#getThreeDFormat--) | Obtiene el formato 3D de la forma. |
| [getTitle()](#getTitle--) | Especifica el título (leyenda) del objeto de forma actual. |
| [getTop()](#getTop--) | Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de píxeles. |
| [getTopCM()](#getTopCM--) | Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de centímetros. |
| [getTopInShape()](#getTopInShape--) | Representa el desplazamiento vertical de la forma desde el borde superior de la forma padre, en unidades de 1/4000 de la altura de la forma padre. |
| [getTopInch()](#getTopInch--) | Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de pulgadas. |
| [getTopToCorner()](#getTopToCorner--) | Obtiene el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles. |
| [getType()](#getType--) | Obtiene el tipo de forma automática. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Obtiene el desplazamiento horizontal de la forma desde la columna de su esquina superior izquierda. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Obtiene el desplazamiento vertical de la forma desde la fila de su esquina superior izquierda. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Representa el índice de columna de la esquina superior izquierda. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Representa el índice de la fila superior. |
| [getWidth()](#getWidth--) | Representa el ancho de la forma, en unidades de píxeles. |
| [getWidthCM()](#getWidthCM--) | Representa el ancho de la forma, en unidades de centímetros. |
| [getWidthInShape()](#getWidthInShape--) | Representa el ancho de la forma, en unidades de 1/4000 de la forma padre. |
| [getWidthInch()](#getWidthInch--) | Representa el ancho de la forma, en unidades de pulgada. |
| [getWidthPt()](#getWidthPt--) | Representa el ancho de la forma, en unidades de punto. |
| [getWidthScale()](#getWidthScale--) | Obtiene la escala de ancho, en unidades de porcentaje del ancho original de la imagen. |
| [getWorksheet()](#getWorksheet--) | Obtiene el objeto [Worksheet](../../com.aspose.cells/worksheet) que contiene esta forma. |
| [getX()](#getX--) | Obtiene el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja, en unidades de píxeles. |
| [getY()](#getY--) | Obtiene el desplazamiento vertical de la forma desde el borde superior de la hoja, en unidades de píxeles. |
| [getZOrderPosition()](#getZOrderPosition--) | Devuelve la posición de una forma en el orden Z. |
| [hasLine()](#hasLine--) | Obtiene si el borde de línea de la forma es visible. |
| [hashCode()](#hashCode--) |  |
| [isAspectRatioLocked()](#isAspectRatioLocked--) | True indica que la relación de aspecto de la forma está bloqueada. |
| [isDecorative()](#isDecorative--) | Indica si el objeto es decorativo. |
| [isEquation()](#isEquation--) | Indica si la forma solo contiene una ecuación. |
| [isFilled()](#isFilled--) | Indica si el formato de relleno es visible. |
| [isFlippedHorizontally()](#isFlippedHorizontally--) | Obtiene si la forma está volteada horizontalmente . |
| [isFlippedVertically()](#isFlippedVertically--) | Obtiene si la forma está volteada verticalmente . |
| [isGroup()](#isGroup--) | Indica si esta forma es una forma de grupo. |
| [isHidden()](#isHidden--) | Indica si el objeto es visible. |
| [isInGroup()](#isInGroup--) | Indica si la forma está agrupada. |
| [isLockAspectRatio()](#isLockAspectRatio--) | True indica que la relación de aspecto de la forma está bloqueada. |
| [isLocked()](#isLocked--) | True indica que el objeto no puede modificarse cuando la hoja está protegida. |
| [isPrintable()](#isPrintable--) | Indica si el objeto es imprimible. |
| [isRichText()](#isRichText--) | Si el texto es o no texto enriquecido. |
| [isSameSetting(Object obj)](#isSameSetting-java.lang.Object-) | Devuelve si la forma es la misma. |
| [isSmartArt()](#isSmartArt--) | Indica si la forma es un arte inteligente. |
| [isTextWrapped()](#isTextWrapped--) | Obtiene el tipo de ajuste de texto de la forma que contiene texto. |
| [isWordArt()](#isWordArt--) | Indica si esta forma es un arte de palabras. |
| [moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)](#moveToRange-int-int-int-int-) | Mueve la forma a un rango especificado. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeActiveXControl()](#removeActiveXControl--) | Eliminar control ActiveX. |
| [removeHyperlink()](#removeHyperlink--) | Elimina el hipervínculo de la forma. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Devuelve o establece la cadena de texto descriptiva (alternativa) del objeto [Shape](../../com.aspose.cells/shape). |
| [setAnchorType(int value)](#setAnchorType-int-) | Establece el tipo del marcador de posición del ancla de la forma. |
| [setAspectRatioLocked(boolean value)](#setAspectRatioLocked-boolean-) | True indica que la relación de aspecto de la forma está bloqueada. |
| [setAutoShapeType(int value)](#setAutoShapeType-int-) | Establece el tipo de forma automática. |
| [setBottom(int value)](#setBottom-int-) | Representa el ancho del desplazamiento vertical de la forma desde la fila de su esquina inferior, en unidades de píxeles. |
| [setCreateId(UUID value)](#setCreateId-java.util.UUID-) | Establece el ID de creación para esta forma. |
| [setDecorative(boolean value)](#setDecorative-boolean-) | Indica si el objeto es decorativo. |
| [setFilled(boolean value)](#setFilled-boolean-) | Indica si el formato de relleno es visible. |
| [setFlippedHorizontally(boolean value)](#setFlippedHorizontally-boolean-) | Establece si la forma está volteada horizontalmente. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Establece si la forma está volteada verticalmente. |
| [setFont(Font value)](#setFont-com.aspose.cells.Font-) | Representa la fuente de la forma. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Establece que el borde de línea de la forma sea visible. |
| [setHeight(int value)](#setHeight-int-) | Representa la altura de la forma, en unidades de píxel. |
| [setHeightCM(double value)](#setHeightCM-double-) | Representa la altura de la forma, en unidades de centímetros. |
| [setHeightInShape(int value)](#setHeightInShape-int-) | Representa el desplazamiento vertical de la forma desde el borde superior de la forma padre, en unidades de 1/4000 de la altura de la forma padre. |
| [setHeightInch(double value)](#setHeightInch-double-) | Representa la altura de la forma, en unidades de pulgadas. |
| [setHeightPt(double value)](#setHeightPt-double-) | Representa la altura de la forma, en unidades de puntos. |
| [setHeightScale(int value)](#setHeightScale-int-) | Establece la escala de altura, en unidades de porcentaje de la altura original de la imagen. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indica si el objeto es visible. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Establece la cadena HTML que contiene datos y algunos formatos en este cuadro de texto. |
| [setInputRange(String value)](#setInputRange-java.lang.String-) | Establece el rango de la hoja de cálculo usado para rellenar el cuadro combinado especificado. |
| [setInputRange(String formula, boolean isR1C1, boolean isLocal)](#setInputRange-java.lang.String-boolean-boolean-) | Establece el rango usado para rellenar el control. |
| [setLeft(int value)](#setLeft-int-) | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxeles. |
| [setLeftCM(double value)](#setLeftCM-double-) | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de centímetros. |
| [setLeftInShape(int value)](#setLeftInShape-int-) | Representa el desplazamiento horizontal de la forma desde el borde izquierdo de la forma padre, en unidades de 1/4000 del ancho de la forma padre. |
| [setLeftInch(double value)](#setLeftInch-double-) | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de pulgadas. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Establece el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Establece el rango de la hoja de cálculo vinculado al valor del control. |
| [setLinkedCell(String formula, boolean isR1C1, boolean isLocal)](#setLinkedCell-java.lang.String-boolean-boolean-) | Establece el rango vinculado al valor del control. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | True indica que la relación de aspecto de la forma está bloqueada. |
| [setLocked(boolean value)](#setLocked-boolean-) | True indica que el objeto no puede modificarse cuando la hoja está protegida. |
| [setLockedProperty(int type, boolean value)](#setLockedProperty-int-boolean-) | Establece la propiedad bloqueada. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Establece el desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Establece el desplazamiento vertical de la forma desde la fila de su esquina inferior derecha. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Representa el índice de columna de la esquina inferior derecha. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Representa el índice de fila de la esquina inferior derecha. |
| [setMacroName(String value)](#setMacroName-java.lang.String-) | Establece el nombre de la macro. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre de la forma. |
| [setPlacement(int value)](#setPlacement-int-) | Representa la forma en que el objeto de dibujo está unido a las celdas debajo de él. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | Indica si el objeto es imprimible. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Indica si la forma es relativa al tamaño original de la imagen. |
| [setRight(int value)](#setRight-int-) | Representa el ancho del desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha, en unidades de píxeles. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Establece la rotación de la forma. |
| [setSoftEdges(double value)](#setSoftEdges-double-) | Establece el radio del desenfoque que se aplicará a los bordes, en unidades de puntos. |
| [setText(String value)](#setText-java.lang.String-) | Establece el texto de esta forma. |
| [setTextDirection(int value)](#setTextDirection-int-) | Establece la dirección del flujo de texto para este objeto. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Establece el tipo de alineación horizontal del texto de la forma. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Establece el tipo de desbordamiento horizontal del texto de la forma que contiene texto. |
| [setTextOptions(TextOptions value)](#setTextOptions-com.aspose.cells.TextOptions-) | Representa las opciones de texto de la forma. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | Establece el tipo de orientación del texto de la forma. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Establece el tipo de forma de texto predefinido. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Establece el tipo de alineación vertical del texto de la forma. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Establece el tipo de desbordamiento vertical del texto de la forma que contiene texto. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Establece el tipo de ajuste de texto de la forma que contiene texto. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Especifica el título (leyenda) del objeto de forma actual. |
| [setTop(int value)](#setTop-int-) | Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de píxeles. |
| [setTopCM(double value)](#setTopCM-double-) | Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de centímetros. |
| [setTopInShape(int value)](#setTopInShape-int-) | Representa el desplazamiento vertical de la forma desde el borde superior de la forma padre, en unidades de 1/4000 de la altura de la forma padre. |
| [setTopInch(double value)](#setTopInch-double-) | Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de pulgadas. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Establece el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Establece el desplazamiento horizontal de la forma desde la columna de su esquina superior izquierda. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Establece el desplazamiento vertical de la forma desde la fila de su esquina superior izquierda. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Representa el índice de columna de la esquina superior izquierda. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Representa el índice de la fila superior. |
| [setWidth(int value)](#setWidth-int-) | Representa el ancho de la forma, en unidades de píxeles. |
| [setWidthCM(double value)](#setWidthCM-double-) | Representa el ancho de la forma, en unidades de centímetros. |
| [setWidthInShape(int value)](#setWidthInShape-int-) | Representa el ancho de la forma, en unidades de 1/4000 de la forma padre. |
| [setWidthInch(double value)](#setWidthInch-double-) | Representa el ancho de la forma, en unidades de pulgada. |
| [setWidthPt(double value)](#setWidthPt-double-) | Representa el ancho de la forma, en unidades de punto. |
| [setWidthScale(int value)](#setWidthScale-int-) | Establece la escala de ancho, en unidades de porcentaje del ancho original de la imagen. |
| [setX(int value)](#setX-int-) | Establece el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo, en unidades de píxeles. |
| [setY(int value)](#setY-int-) | Establece el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Devuelve la posición de una forma en el orden Z. |
| [toFrontOrBack(int orders)](#toFrontOrBack-int-) | Mueve la forma al frente o la envía al fondo. |
| [toImage(OutputStream stream, ImageFormat imageFormat)](#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-) | Crea la imagen de la forma y la guarda en un flujo en el formato especificado. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Guarda la forma en un flujo. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Guarda la forma en un archivo. |
| [toString()](#toString--) |  |
| [updateSelectedValue()](#updateSelectedValue--) | Actualiza el valor seleccionado con el valor de la celda vinculada. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public Hyperlink addHyperlink(String address)
```


Agrega un hipervínculo a la forma.

**Example**

```
         Hyperlink hyperlink = shape.addHyperlink("https://www.aspose.com/");
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dirección | java.lang.String | Dirección del hipervínculo. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - Returns the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Mueve la imagen a la esquina superior derecha.

**Example**

```
         shape.alignTopRightCorner(2, 5);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | el índice de fila. |
| rightColumn | int | el índice de la columna. |

### calculateTextSize() {#calculateTextSize--}
```
public int[] calculateTextSize()
```


Recalcular el área de texto

**Example**

```
         //The size of the text area is:w=size[0],h=size[1]
         int[] size = shape.calculateTextSize();
```

**Returns:**
int[] - Tamaño del texto en una matriz (ancho y alto).
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Devuelve un objeto Characters que representa un rango de caracteres dentro del texto.

**Remarks**

Este método solo funciona en una forma con título.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | int | El índice del inicio del carácter. |
| length | int | El número de caracteres. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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
### fitToTextSize() {#fitToTextSize--}
```
public void fitToTextSize()
```


Recalcula un área de texto adecuada para mostrar todo el contenido del texto.

**Example**

```
         if (shape.getName().startsWith("Your traget"))
         {
             shape.fitToTextSize();
         }
```

### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


Da formato a algunos caracteres con la configuración de fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | int | El índice de inicio. |
| length | int | La longitud. |
| font | [Font](../../com.aspose.cells/font) | La configuración de la fuente. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | La bandera de la configuración de la fuente. |

### getActiveXControl() {#getActiveXControl--}
```
public ActiveXControl getActiveXControl()
```


Obtiene el control ActiveX.

**Example**

```
         if(shape.getActiveXControl() != null)
         {
             CheckBoxActiveXControl checkBox1 = (CheckBoxActiveXControl)shape.getActiveXControl();
             //The font name of CheckBox
             String fontName = checkBox1.getFont().getName();
         }
```

**Returns:**
[ActiveXControl](../../com.aspose.cells/activexcontrol)
### getActualBox() {#getActualBox--}
```
public float[] getActualBox()
```


Obtenga la posición y el tamaño reales de la forma (después de aplicar rotación, volteo, etc.)

**Remarks**

Nota: La interfaz no está completamente funcional, especialmente la información de ubicación no es correcta. Se recomienda no usar esta interfaz hasta que la función esté completa.

**Example**

```
         float[] box = shape.getActualBox();
         System.out.println("x = " + box[0]);
         System.out.println("y = " + box[1]);
         System.out.println("w = " + box[2]);
         System.out.println("h = " + box[3]);
```

**Returns:**
float[] - Devuelve la posición y el tamaño en el orden x, y, w, h
### getActualLowerRightRow() {#getActualLowerRightRow--}
```
public int getActualLowerRightRow()
```


Obtenga la fila inferior real.

**Example**

```
         int rRow = shape.getActualLowerRightRow();
```

**Returns:**
int
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Devuelve o establece la cadena de texto descriptiva (alternativa) del objeto [Shape](../../com.aspose.cells/shape).

**Example**

```
         shape.setAlternativeText("a rectangle");
```

**Returns:**
java.lang.String
### getAnchorType() {#getAnchorType--}
```
public int getAnchorType()
```


Obtiene el tipo del marcador de posición del ancla de la forma.

Ver [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

**Example**

```
         if (shape.getAnchorType() == ShapeAnchorType.ONE_CELL_ANCHOR)
             shape.setAnchorType(ShapeAnchorType.TWO_CELL_ANCHOR);
```

**Returns:**
int
### getAutoShapeType() {#getAutoShapeType--}
```
public int getAutoShapeType()
```


Obtiene el tipo de forma automática.

Ver [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         if (shape.getAutoShapeType() == com.aspose.cells.AutoShapeType.UNKNOWN)
             shape.setAutoShapeType(com.aspose.cells.AutoShapeType.RECTANGLE);
```

**Returns:**
int
### getBottom() {#getBottom--}
```
public int getBottom()
```


Representa el ancho del desplazamiento vertical de la forma desde la fila de su esquina inferior, en unidades de píxeles.

**Example**

```
         if (shape.getBottom() == 3)
             shape.setBottom(1);
```

**Returns:**
int
### getCharacters() {#getCharacters--}
```
public ArrayList getCharacters()
```


Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método Shape.GetRichFormattings(). Este método será eliminado 12 meses después, a partir de noviembre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Returns:**
java.util.ArrayList - Todos los objetos Characters
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConnectionPoints() {#getConnectionPoints--}
```
public float[][] getConnectionPoints()
```


Obtiene los puntos de conexión

**Example**

```
         float[][] points = shape.getConnectionPoints();
```

**Returns:**
float[][] - pares [X,Y] del punto de conexión. Cada elemento es una matriz float[2], [0] representa x y [1] representa y.
### getControlData() {#getControlData--}
```
public byte[] getControlData()
```


Obtiene los datos del control.

**Example**

```
         if(shape.getControlData() == null)
             System.out.println("No data.");
```

**Returns:**
byte[]
### getCreateId() {#getCreateId--}
```
public UUID getCreateId()
```


Obtiene el id de creación para esta forma.

**Example**

```
         System.out.println(shape.getCreateId());
         java.util.UUID g = java.util.UUID.randomUUID();
         shape.setCreateId(g);
         System.out.println(shape.getCreateId());
```

**Returns:**
java.util.UUID
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Devuelve un objeto [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--) que contiene las propiedades de formato de relleno para la forma especificada.

**Example**

```
         FillFormat fillFmt = shape.getFill();
```

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getFillFormat() {#getFillFormat--}
```
public MsoFillFormat getFillFormat()
```


Devuelve un objeto MsoFillFormat que contiene las propiedades de formato de relleno para la forma especificada.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Fill. Esta propiedad será eliminada 12 meses después, a partir de julio de 2016. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
[MsoFillFormat](../../com.aspose.cells/msofillformat)
### getFont() {#getFont--}
```
public Font getFont()
```


Representa la fuente de la forma.

**Example**

```
         Font font = shape.getFont();
         font.setName("Arial");
         font.setSize(12);
         font.setColor(Color.getRed());
```

**Returns:**
[Font](../../com.aspose.cells/font)
### getFormatPicture() {#getFormatPicture--}
```
public MsoFormatPicture getFormatPicture()
```


Obtiene las opciones del formato de imagen.

**Example**

```
         MsoFormatPicture msoFormatPicture = shape.getFormatPicture();
```

**Returns:**
[MsoFormatPicture](../../com.aspose.cells/msoformatpicture)
### getGeometry() {#getGeometry--}
```
public Geometry getGeometry()
```


Obtiene la geometría

**Example**

```
         if (shape.getGeometry() != null &&shape.getGeometry().getShapeAdjustValues().getCount() == 0)
             System.out.println("No geometry path.");
```

**Returns:**
[Geometry](../../com.aspose.cells/geometry)
### getGlow() {#getGlow--}
```
public GlowEffect getGlow()
```


Representa un objeto [GlowEffect](../../com.aspose.cells/gloweffect) que especifica el efecto de resplandor para el elemento del gráfico o la forma.

**Example**

```
         GlowEffect glowEffect = shape.getGlow();
```

**Returns:**
[GlowEffect](../../com.aspose.cells/gloweffect)
### getGroup() {#getGroup--}
```
public GroupShape getGroup()
```


Obtiene el grupo de formas que contiene esta forma.

**Example**

```
         GroupShape groupShape = shape.getGroup();
```

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Representa la altura de la forma, en unidades de píxel.

**Example**

```
         if (shape.getHeight() == 3)
             shape.setHeight(1);
```

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


Representa la altura de la forma, en unidades de centímetros.

**Example**

```
         if (shape.getHeightCM() == 3)
             shape.setHeightCM(1);
```

**Returns:**
double
### getHeightInShape() {#getHeightInShape--}
```
public int getHeightInShape()
```


Representa el desplazamiento vertical de la forma desde el borde superior de la forma padre, en unidades de 1/4000 de la altura de la forma padre.

**Remarks**

Solo se aplica cuando esta forma está en el grupo o en el gráfico.

**Example**

```
         if (shape.isInGroup() &&shape.getHeightInShape() == 4000)
             shape.setHeightInShape(2000);
```

**Returns:**
int
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


Representa la altura de la forma, en unidades de pulgadas.

**Example**

```
         if (shape.getHeightInch() == 3)
             shape.setHeightInch(1);
```

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


Representa la altura de la forma, en unidades de puntos.

**Example**

```
         if (shape.getHeightPt() == 3)
             shape.setHeightPt(1);
```

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


Obtiene la escala de altura, en unidades de porcentaje de la altura original de la imagen. Si la forma no es una imagen, la propiedad HeightScale solo devuelve 100;

**Example**

```
         if (shape.getHeightScale() == 3)
             shape.setHeightScale(1);
```

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


Obtiene la cadena HTML que contiene datos y algunos formatos en este cuadro de texto.

**Example**

```
         String html = shape.getHtmlText();
         if(html == null || "".equals(html))
         {
             shape.setHtmlText("<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>");
         }
```

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public Hyperlink getHyperlink()
```


Obtiene el hipervínculo de la forma.

**Example**

```
         Hyperlink hyperlink = shape.getHyperlink();
```

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink)
### getId() {#getId--}
```
public int getId()
```


Obtiene el identificador de esta forma.

**Example**

```
         int id = shape.getId();
```

**Returns:**
int
### getInputRange() {#getInputRange--}
```
public String getInputRange()
```


Obtiene el rango de hoja de cálculo utilizado para rellenar el cuadro combinado especificado.

**Example**

```
         if (shape.getInputRange().equals("$B$6:$B10"))
             shape.setInputRange("$A$1:$A$5");
```

**Returns:**
java.lang.String
### getInputRange(boolean isR1C1, boolean isLocal) {#getInputRange-boolean-boolean-}
```
public String getInputRange(boolean isR1C1, boolean isLocal)
```


Obtiene el rango utilizado para rellenar el control.

**Example**

```
         String range = shape.getInputRange(false, true);
         //If successful, a value like "$A$1:$A$3" will be returned
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |

**Returns:**
java.lang.String - El rango utilizado para rellenar el control.
### getLeft() {#getLeft--}
```
public int getLeft()
```


Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxeles.

**Example**

```
         if (shape.getLeft() == 3)
             shape.setLeft(1);
```

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de centímetros.

**Example**

```
         if (shape.getLeftCM() == 3)
             shape.setLeftCM(1);
```

**Returns:**
double
### getLeftInShape() {#getLeftInShape--}
```
public int getLeftInShape()
```


Representa el desplazamiento horizontal de la forma desde el borde izquierdo de la forma padre, en unidades de 1/4000 del ancho de la forma padre.

**Remarks**

Solo se aplica cuando esta forma está en el grupo o en el gráfico.

**Example**

```
         if (shape.isInGroup() &&shape.getLeftInShape() == 2000)
             shape.setLeftInShape(4000);
```

**Returns:**
int
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de pulgadas.

**Example**

```
         if (shape.getLeftInch() == 3)
             shape.setLeftInch(1);
```

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Obtiene el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo.

**Example**

```
         if (shape.getLeftToCorner() == 3)
             shape.setLeftToCorner(1);
```

**Returns:**
int
### getLine() {#getLine--}
```
public LineFormat getLine()
```


Obtiene el estilo de línea

**Example**

```
         LineFormat lineFmt = shape.getLine();
```

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getLineFormat() {#getLineFormat--}
```
public MsoLineFormat getLineFormat()
```


Devuelve un objeto MsoLineFormat que contiene las propiedades de formato de línea para la forma especificada.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Shape.Line. Esta propiedad será eliminada 12 meses después desde julio de 2016. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
[MsoLineFormat](../../com.aspose.cells/msolineformat)
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Obtiene el rango de la hoja de cálculo vinculado al valor del control.

**Example**

```
         if (shape.getLinkedCell().equals("$B$6"))
         {
             shape.setLinkedCell("A1");
         }
         shape.updateSelectedValue();
```

**Returns:**
java.lang.String
### getLinkedCell(boolean isR1C1, boolean isLocal) {#getLinkedCell-boolean-boolean-}
```
public String getLinkedCell(boolean isR1C1, boolean isLocal)
```


Obtiene el rango vinculado al valor del control.

**Example**

```
         //You may get results like '$A$1'
         String link = shape.getLinkedCell(false, false);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |

**Returns:**
java.lang.String - El rango vinculado al valor del control.
### getLockedProperty(int type) {#getLockedProperty-int-}
```
public boolean getLockedProperty(int type)
```


Obtiene el valor de la propiedad locked.

**Example**

```
         int noAdjustHandles = 0;
         if (shape.getLockedProperty(ShapeLockType.ADJUST_HANDLES))
             noAdjustHandles = 1;
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). El tipo de la propiedad de bloqueo de la forma. |

**Returns:**
boolean - Devuelve el valor de la propiedad locked.
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


Obtiene el desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha.

**Remarks**

El rango de valores es de 0 a 1024.

**Example**

```
         if (shape.getLowerDeltaX() == 3)
             shape.setLowerDeltaX(1);
```

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


Obtiene el desplazamiento vertical de la forma desde la fila de su esquina inferior derecha.

**Remarks**

El rango de valores es de 0 a 256.

**Example**

```
         if (shape.getLowerDeltaY() == 3)
             shape.setLowerDeltaY(1);
```

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


Representa el índice de columna de la esquina inferior derecha.

**Example**

```
         if (shape.getLowerRightColumn() == 3)
             shape.setLowerRightColumn(1);
```

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


Representa el índice de fila de la esquina inferior derecha.

**Example**

```
         if (shape.getLowerRightRow() == 3)
             shape.setLowerRightRow(1);
```

**Returns:**
int
### getMacroName() {#getMacroName--}
```
public String getMacroName()
```


Obtiene el nombre de la macro.

**Example**

```
         //Sets the name of macro.
         shape.setMacroName("DoWork()");
```

**Returns:**
java.lang.String
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


Obtiene el tipo de dibujo.

Ver [MsoDrawingType](../../com.aspose.cells/msodrawingtype).

**Example**

```
         /*Aspose.Cells.Drawing.MsoDrawingType*/int msoDrawingType = shape.getMsoDrawingType();
```

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre de la forma.

**Example**

```
         shape.setName("shape1");
```

**Returns:**
java.lang.String
### getPaths() {#getPaths--}
```
public ShapePathCollection getPaths()
```


Obtiene las rutas de una forma geométrica personalizada.

**Example**

```
         //Returns non-null if there is a path to the custom geometry
         if(shape.getPaths() == null)
             System.out.println("No custom geometry path.");
```

**Returns:**
[ShapePathCollection](../../com.aspose.cells/shapepathcollection)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Representa la forma en que el objeto de dibujo está unido a las celdas debajo de él. La propiedad controla la ubicación de un objeto en una hoja de cálculo.

Ver [PlacementType](../../com.aspose.cells/placementtype).

**Example**

```
         if (shape.getPlacement() == PlacementType.MOVE)
             shape.setPlacement(PlacementType.MOVE_AND_SIZE);
```

**Returns:**
int
### getReflection() {#getReflection--}
```
public ReflectionEffect getReflection()
```


Representa un objeto [ReflectionEffect](../../com.aspose.cells/reflectioneffect) que especifica el efecto de reflexión para el elemento de gráfico o forma.

**Example**

```
         ReflectionEffect reflectionEffect = shape.getReflection();
```

**Returns:**
[ReflectionEffect](../../com.aspose.cells/reflectioneffect)
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


Indica si la forma es relativa al tamaño original de la imagen.

**Example**

```
         if(shape.getRelativeToOriginalPictureSize())
             shape.setRelativeToOriginalPictureSize(false);
```

**Returns:**
boolean
### getResultOfSmartArt() {#getResultOfSmartArt--}
```
public GroupShape getResultOfSmartArt()
```


Convirtiendo arte inteligente a formas agrupadas.

**Example**

```
         if(shape.isSmartArt())
         {
             GroupShape groupShape = shape.getResultOfSmartArt();
         }
```

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape)
### getRichFormattings() {#getRichFormattings--}
```
public FontSetting[] getRichFormattings()
```


Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto.

**Example**

```
         FontSetting[] list = shape.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - Todos los objetos Characters
### getRight() {#getRight--}
```
public int getRight()
```


Representa el ancho del desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha, en unidades de píxeles.

**Example**

```
         if (shape.getRight() == 3)
             shape.setRight(1);
```

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


Obtiene la rotación de la forma.

**Example**

```
         //Gets rotation angle of the shape.
         double angle = shape.getRotationAngle() ;
 
         //Gets rotation angle of the shape.
          shape.setRotationAngle(60);
```

**Returns:**
double
### getShadowEffect() {#getShadowEffect--}
```
public ShadowEffect getShadowEffect()
```


Representa un objeto [ShadowEffect](../../com.aspose.cells/shadoweffect) que especifica el efecto de sombra para el elemento de gráfico o forma.

**Example**

```
         ShadowEffect shadowEffect = shape.getShadowEffect();
```

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSoftEdges() {#getSoftEdges--}
```
public double getSoftEdges()
```


Obtiene el radio del desenfoque que se aplicará a los bordes, en unidades de puntos.

**Example**

```
         shape.setSoftEdges(0.5d);
```

**Returns:**
double
### getSpid() {#getSpid--}
```
public String getSpid()
```


Especifica un identificador de cadena opcional que una aplicación puede usar para identificar la forma particular.

**Example**

```
         String spid = shape.getSpid();
```

**Returns:**
java.lang.String
### getSpt() {#getSpt--}
```
public int getSpt()
```


Especifica un número opcional que una aplicación puede usar para asociar la forma particular con un tipo de forma definido.

**Example**

```
         int spt = shape.getSpt();
```

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Obtiene el texto de esta forma.

**Example**

```
         if(shape.getText() == null)
             shape.setText("This is a test.");
```

**Returns:**
java.lang.String
### getTextBody() {#getTextBody--}
```
public FontSettingCollection getTextBody()
```


Obtiene la configuración del texto de la forma.

**Example**

```
         FontSettingCollection fontSettingCollection = shape.getTextBody();
         fontSettingCollection.setText("This is a test.");
```

**Returns:**
[FontSettingCollection](../../com.aspose.cells/fontsettingcollection)
### getTextBoxOptions() {#getTextBoxOptions--}
```
public TextBoxOptions getTextBoxOptions()
```


Obtiene la información de texto en la forma

**Example**

```
         TextBoxOptions textBoxOpt = shape.getTextBoxOptions();
         textBoxOpt.setShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType.LEFT);
         textBoxOpt.setTopMarginPt(0.2d);
         textBoxOpt.setLeftMarginPt(0.2d);
         textBoxOpt.setRightMarginPt(0.2d);
         textBoxOpt.setBottomMarginPt(0.2d);
```

**Returns:**
[TextBoxOptions](../../com.aspose.cells/textboxoptions)
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Obtiene la dirección del flujo de texto para este objeto.

Ver [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Example**

```
         if (shape.getTextDirection() == com.aspose.cells.TextDirectionType.CONTEXT)
             shape.setTextDirection(com.aspose.cells.TextDirectionType.LEFT_TO_RIGHT);
```

**Returns:**
int
### getTextEffect() {#getTextEffect--}
```
public TextEffectFormat getTextEffect()
```


Devuelve un objeto TextEffectFormat que contiene propiedades de formato de efectos de texto para la forma especificada. Se aplica a objetos Shape que representan WordArt.

**Example**

```
         if(shape.isWordArt())
         {
             TextEffectFormat textEffectFormat = shape.getTextEffect();
         }
```

**Returns:**
[TextEffectFormat](../../com.aspose.cells/texteffectformat)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


Obtiene el tipo de alineación horizontal del texto de la forma.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Example**

```
         if (shape.getTextHorizontalAlignment() == com.aspose.cells.TextAlignmentType.BOTTOM)
             shape.setTextHorizontalAlignment(com.aspose.cells.TextAlignmentType.CENTER);
```

**Returns:**
int
### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}
```
public int getTextHorizontalOverflow()
```


Obtiene el tipo de desbordamiento horizontal del texto de la forma que contiene texto.

Ver [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         if (shape.getTextHorizontalOverflow() == com.aspose.cells.TextOverflowType.CLIP)
             shape.setTextHorizontalOverflow(com.aspose.cells.TextOverflowType.OVERFLOW);
```

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Representa las opciones de texto de la forma.

**Example**

```
         TextOptions opt = shape.getTextOptions();
         opt.setColor(Color.getBlue());
         opt.setSize(8);
```

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextOrientationType() {#getTextOrientationType--}
```
public int getTextOrientationType()
```


Obtiene el tipo de orientación del texto de la forma.

Ver [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Example**

```
         if (shape.getTextOrientationType() == com.aspose.cells.TextOrientationType.NO_ROTATION)
             shape.setTextOrientationType(com.aspose.cells.TextOrientationType.TOP_TO_BOTTOM);
```

**Returns:**
int
### getTextShapeType() {#getTextShapeType--}
```
public int getTextShapeType()
```


Obtiene el tipo de forma de texto predefinido.

Ver [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         if (shape.getTextShapeType() == com.aspose.cells.AutoShapeType.UNKNOWN)
             shape.setTextShapeType(com.aspose.cells.AutoShapeType.RECTANGLE);
```

**Returns:**
int
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


Obtiene el tipo de alineación vertical del texto de la forma.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Example**

```
         if (shape.getTextVerticalAlignment() == com.aspose.cells.TextAlignmentType.BOTTOM)
             shape.setTextVerticalAlignment(com.aspose.cells.TextAlignmentType.CENTER);
```

**Returns:**
int
### getTextVerticalOverflow() {#getTextVerticalOverflow--}
```
public int getTextVerticalOverflow()
```


Obtiene el tipo de desbordamiento vertical del texto de la forma que contiene texto.

Ver [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         if (shape.getTextVerticalOverflow() == com.aspose.cells.TextOverflowType.CLIP)
             shape.setTextVerticalOverflow(com.aspose.cells.TextOverflowType.OVERFLOW);
```

**Returns:**
int
### getThreeDFormat() {#getThreeDFormat--}
```
public ThreeDFormat getThreeDFormat()
```


Obtiene el formato 3D de la forma.

**Example**

```
         ThreeDFormat threeDFormat = shape.getThreeDFormat();
```

**Returns:**
[ThreeDFormat](../../com.aspose.cells/threedformat)
### getTitle() {#getTitle--}
```
public String getTitle()
```


Especifica el título (leyenda) del objeto de forma actual.

**Example**

```
         shape.setTitle("title1");
```

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de píxeles.

**Remarks**

Si la forma está en el gráfico, representa el desplazamiento vertical de la forma desde su borde superior.

**Example**

```
         if (shape.getTop() == 3)
             shape.setTop(1);
```

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de centímetros.

**Example**

```
         if (shape.getTopCM() == 3)
             shape.setTopCM(1);
```

**Returns:**
double
### getTopInShape() {#getTopInShape--}
```
public int getTopInShape()
```


Representa el desplazamiento vertical de la forma desde el borde superior de la forma padre, en unidades de 1/4000 de la altura de la forma padre.

**Remarks**

Solo se aplica cuando esta forma está en el grupo o en el gráfico.

**Example**

```
         if (shape.isInGroup() &&shape.getTopInShape() == 8000)
             shape.setTopInShape(4000);
```

**Returns:**
int
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de pulgadas.

**Example**

```
         if (shape.getTopInch() == 3)
             shape.setTopInch(1);
```

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Obtiene el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles.

**Example**

```
         if (shape.getTopToCorner() == 3)
             shape.setTopToCorner(1);
```

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Obtiene el tipo de forma automática.

Ver [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         /*Aspose.Cells.Drawing.AutoShapeType*/int autoShapeType = shape.getType();
```

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


Obtiene el desplazamiento horizontal de la forma desde la columna de su esquina superior izquierda.

**Remarks**

El rango de valores es de 0 a 1024.

**Example**

```
         if (shape.getUpperDeltaX() == 3)
             shape.setUpperDeltaX(1);
```

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


Obtiene el desplazamiento vertical de la forma desde la fila de su esquina superior izquierda.

**Remarks**

El rango de valores es de 0 a 256.

**Example**

```
         if (shape.getUpperDeltaY() == 3)
             shape.setUpperDeltaY(1);
```

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Representa el índice de columna de la esquina superior izquierda.

**Example**

```
         if (shape.getUpperLeftColumn() == 3)
             shape.setUpperLeftColumn(1);
```

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Representa el índice de la fila superior.

**Remarks**

Si la forma está dentro de otra forma o en el grupo, UpperLeftRow será ignorado.

**Example**

```
         if (shape.getUpperLeftRow() == 3)
             shape.setUpperLeftRow(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Representa el ancho de la forma, en unidades de píxeles.

**Example**

```
         if (shape.getWidth() == 3)
             shape.setWidth(1);
```

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


Representa el ancho de la forma, en unidades de centímetros.

**Example**

```
         if (shape.getWidthCM() == 3)
             shape.setWidthCM(1);
```

**Returns:**
double
### getWidthInShape() {#getWidthInShape--}
```
public int getWidthInShape()
```


Representa el ancho de la forma, en unidades de 1/4000 de la forma padre.

**Remarks**

Solo se aplica cuando esta forma está en el grupo o en el gráfico.

**Example**

```
         if (shape.isInGroup() &&shape.getWidthInShape() == 2000)
             shape.setWidthInShape(4000);
```

**Returns:**
int
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


Representa el ancho de la forma, en unidades de pulgada.

**Example**

```
         if (shape.getWidthInch() == 3)
             shape.setWidthInch(1);
```

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


Representa el ancho de la forma, en unidades de punto.

**Example**

```
         if (shape.getWidthPt() == 3)
             shape.setWidthPt(1);
```

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


Obtiene la escala de ancho, en unidades de porcentaje del ancho original de la imagen. Si la forma no es una imagen, la propiedad WidthScale solo devuelve 100;

**Example**

```
         if (shape.getWidthScale() == 3)
             shape.setWidthScale(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Obtiene el objeto [Worksheet](../../com.aspose.cells/worksheet) que contiene esta forma.

**Example**

```
         Worksheet worksheet = shape.getWorksheet();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getX() {#getX--}
```
public int getX()
```


Obtiene el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja, en unidades de píxeles.

**Example**

```
         if (shape.getX() == 3)
             shape.setX(1);
```

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Obtiene el desplazamiento vertical de la forma desde el borde superior de la hoja, en unidades de píxeles.

**Example**

```
         if (shape.getY() == 3)
             shape.setY(1);
```

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Devuelve la posición de una forma en el orden Z.

**Example**

```
         shape.setZOrderPosition(3);
```

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


Obtiene si el borde de línea de la forma es visible.

**Example**

```
         if(shape.hasLine() == false)
             shape.setHasLine(true);
```

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAspectRatioLocked() {#isAspectRatioLocked--}
```
public boolean isAspectRatioLocked()
```


True indica que la relación de aspecto de la forma está bloqueada.

**Remarks**

Solo para imágenes y objetos Ole.

**Example**

```
         shape.setAspectRatioLocked(false);
```

**Returns:**
boolean
### isDecorative() {#isDecorative--}
```
public boolean isDecorative()
```


Indica si el objeto es decorativo.

**Example**

```
         if (!shape.isDecorative())
             shape.setDecorative(true);
```

**Returns:**
boolean
### isEquation() {#isEquation--}
```
public boolean isEquation()
```


Indica si la forma solo contiene una ecuación.

**Example**

```
         //If true,the shape only contains an equation.
         if(shape.isEquation())
         {
             //The shape contains only an equation
         }
```

**Returns:**
boolean
### isFilled() {#isFilled--}
```
public boolean isFilled()
```


Indica si el formato de relleno es visible.

**Example**

```
         if(shape.isFilled() == false)
             shape.setFilled(true);
```

**Returns:**
boolean
### isFlippedHorizontally() {#isFlippedHorizontally--}
```
public boolean isFlippedHorizontally()
```


Obtiene si la forma está volteada horizontalmente .

**Example**

```
         if(shape.isFlippedHorizontally() == false)
             shape.setFlippedHorizontally(true);
```

**Returns:**
boolean
### isFlippedVertically() {#isFlippedVertically--}
```
public boolean isFlippedVertically()
```


Obtiene si la forma está volteada verticalmente .

**Example**

```
         if(shape.isFlippedVertically() == false)
             shape.setFlippedVertically(true);
```

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


Indica si esta forma es una forma de grupo.

**Example**

```
         if(shape.isGroup())
         {
             //This shape is a group.
         }
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indica si el objeto es visible.

**Example**

```
         shape.setHidden(false);
```

**Returns:**
boolean
### isInGroup() {#isInGroup--}
```
public boolean isInGroup()
```


Indica si la forma está agrupada.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


True indica que la relación de aspecto de la forma está bloqueada.

**Remarks**

Solo para imágenes y objetos Ole. NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Shape.IsAspectRatioLocked. Esta propiedad será eliminada 12 meses después a partir de julio de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Example**

```
         shape.setHidden(false);
```

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


True indica que el objeto no puede modificarse cuando la hoja está protegida. Tenga en cuenta que este valor solo tiene sentido si la hoja de cálculo o los objetos en la hoja de cálculo están protegidos.

**Example**

```
         //Sets the specified shape to unlocked state
         if (shape.getWorksheet().isProtected() &&shape.isLocked())
         {
             shape.setLocked(false);
         }
 
         //Sets the specified shape to a locked state
         if (shape.getWorksheet().isProtected() &&!shape.isLocked())
         {
             shape.setLocked(true);
         }
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


Indica si el objeto es imprimible. Si False, esta forma no se imprimirá al imprimir.

**Example**

```
         if(shape.isPrintable())
             shape.setPrintable(false);
```

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


Si el texto es o no texto enriquecido.

**Example**

```
         if(shape.isRichText())
             System.out.println("The text is rich text.");
```

**Returns:**
boolean
### isSameSetting(Object obj) {#isSameSetting-java.lang.Object-}
```
public boolean isSameSetting(Object obj)
```


Devuelve si la forma es la misma.

**Example**

```
         if (shape.isSameSetting(shape))
             System.out.println("Two objects the same.");
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### isSmartArt() {#isSmartArt--}
```
public boolean isSmartArt()
```


Indica si la forma es un arte inteligente.

**Remarks**

Solo para archivo ooxml.

**Example**

```
         //if true,the shape is a smart art.
         if(shape.isSmartArt())
         {
             //The shape is SmartArt object.
         }
```

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Obtiene el tipo de ajuste de texto de la forma que contiene texto.

**Example**

```
         if (shape.isTextWrapped())
             shape.setTextWrapped(!shape.isTextWrapped());
```

**Returns:**
boolean
### isWordArt() {#isWordArt--}
```
public boolean isWordArt()
```


Indica si esta forma es un arte de palabras.

**Remarks**

Solo para la forma Legacy de archivo xls.

**Example**

```
         if(shape.isWordArt())
         {
             //This shape is a WordArt object.
         }
```

**Returns:**
boolean
### moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Mueve la forma a un rango especificado.

**Example**

```
         shape.moveToRange(12, 3, 13, 5);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| bottomRow | int | Índice de fila inferior derecha |
| rightColumn | int | Índice de columna inferior derecha |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeActiveXControl() {#removeActiveXControl--}
```
public void removeActiveXControl()
```


Eliminar control ActiveX.

**Example**

```
         if(shape.getActiveXControl() != null)
         {
             shape.removeActiveXControl();
         }
```

### removeHyperlink() {#removeHyperlink--}
```
public void removeHyperlink()
```


Elimina el hipervínculo de la forma.

**Example**

```
         shape.removeHyperlink();
```

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Devuelve o establece la cadena de texto descriptiva (alternativa) del objeto [Shape](../../com.aspose.cells/shape).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setAnchorType(int value) {#setAnchorType-int-}
```
public void setAnchorType(int value)
```


Establece el tipo del marcador de posición del ancla de la forma.

Ver [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setAspectRatioLocked(boolean value) {#setAspectRatioLocked-boolean-}
```
public void setAspectRatioLocked(boolean value)
```


True indica que la relación de aspecto de la forma está bloqueada.

**Remarks**

Solo para imágenes y objetos Ole.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutoShapeType(int value) {#setAutoShapeType-int-}
```
public void setAutoShapeType(int value)
```


Establece el tipo de forma automática.

Ver [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


Representa el ancho del desplazamiento vertical de la forma desde la fila de su esquina inferior, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCreateId(UUID value) {#setCreateId-java.util.UUID-}
```
public void setCreateId(UUID value)
```


Establece el ID de creación para esta forma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.UUID |  |

### setDecorative(boolean value) {#setDecorative-boolean-}
```
public void setDecorative(boolean value)
```


Indica si el objeto es decorativo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFilled(boolean value) {#setFilled-boolean-}
```
public void setFilled(boolean value)
```


Indica si el formato de relleno es visible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFlippedHorizontally(boolean value) {#setFlippedHorizontally-boolean-}
```
public void setFlippedHorizontally(boolean value)
```


Establece si la forma está volteada horizontalmente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


Establece si la forma está volteada verticalmente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFont(Font value) {#setFont-com.aspose.cells.Font-}
```
public void setFont(Font value)
```


Representa la fuente de la forma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Font](../../com.aspose.cells/font) |  |

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


Representa la altura de la forma, en unidades de centímetros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setHeightInShape(int value) {#setHeightInShape-int-}
```
public void setHeightInShape(int value)
```


Representa el desplazamiento vertical de la forma desde el borde superior de la forma padre, en unidades de 1/4000 de la altura de la forma padre.

**Remarks**

Solo se aplica cuando esta forma está en el grupo o en el gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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


Establece la cadena HTML que contiene datos y algunos formatos en este cuadro de texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setInputRange(String value) {#setInputRange-java.lang.String-}
```
public void setInputRange(String value)
```


Establece el rango de la hoja de cálculo usado para rellenar el cuadro combinado especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setInputRange(String formula, boolean isR1C1, boolean isLocal) {#setInputRange-java.lang.String-boolean-boolean-}
```
public void setInputRange(String formula, boolean isR1C1, boolean isLocal)
```


Establece el rango usado para rellenar el control.

**Example**

```
         //After executing the code below, a ListBox object is created in the generated file. When the selected option is clicked, the selected value is displayed in cell A12.
 
         for (int i = 0; i? ++i)
         {
             Cell cell = book.getWorksheets().get(0).getCells().get(i, 0);
             cell.setValue(i + 1);
         }
 
         //Create a ListBox object
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
 
         //Form Controls
         Shape listBox = book.getWorksheets().get(0).getShapes().addListBox(2, 0, 2, 0, 130, 130);
 
         //Sets the range used to fill the control.
         listBox.setInputRange("$A$1:$A$6", false, false);
 
         //Sets the range linked to the control's value.
         listBox.setLinkedCell("$A$12", false, true);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | El rango usado para rellenar el control. |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |

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

### setLeftInShape(int value) {#setLeftInShape-int-}
```
public void setLeftInShape(int value)
```


Representa el desplazamiento horizontal de la forma desde el borde izquierdo de la forma padre, en unidades de 1/4000 del ancho de la forma padre.

**Remarks**

Solo se aplica cuando esta forma está en el grupo o en el gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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


Establece el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo.

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

### setLinkedCell(String formula, boolean isR1C1, boolean isLocal) {#setLinkedCell-java.lang.String-boolean-boolean-}
```
public void setLinkedCell(String formula, boolean isR1C1, boolean isLocal)
```


Establece el rango vinculado al valor del control.

**Example**

```
         //After executing the code below, a ScrollBar object is created in the generated file. As you drag the slider, the value is displayed in cell A12.
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape scrollBar = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ScrollBar,2, 0, 2, 0, 30, 130);
 
         //Form Controls
         Shape scrollBar = book.getWorksheets().get(0).getShapes().addScrollBar(2, 0, 2, 0, 130, 30);
 
         //Sets the range linked to the control's value.
         scrollBar.setLinkedCell("$A$12", false, true);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | El rango vinculado al valor del control. |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


True indica que la relación de aspecto de la forma está bloqueada.

**Remarks**

Solo para imágenes y objetos Ole. NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Shape.IsAspectRatioLocked. Esta propiedad será eliminada 12 meses después a partir de julio de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


True indica que el objeto no puede modificarse cuando la hoja está protegida. Tenga en cuenta que este valor solo tiene sentido si la hoja de cálculo o los objetos en la hoja de cálculo están protegidos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLockedProperty(int type, boolean value) {#setLockedProperty-int-boolean-}
```
public void setLockedProperty(int type, boolean value)
```


Establece la propiedad bloqueada.

**Example**

```
         shape.setLockedProperty(ShapeLockType.ADJUST_HANDLES, true);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). El tipo bloqueado. |
| valor | boolean | El valor de la propiedad. |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


Establece el desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha.

**Remarks**

El rango de valores es de 0 a 1024.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


Establece el desplazamiento vertical de la forma desde la fila de su esquina inferior derecha.

**Remarks**

El rango de valores es de 0 a 256.

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

### setMacroName(String value) {#setMacroName-java.lang.String-}
```
public void setMacroName(String value)
```


Establece el nombre de la macro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Establece el nombre de la forma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Representa la forma en que el objeto de dibujo está unido a las celdas debajo de él. La propiedad controla la ubicación de un objeto en una hoja de cálculo.

Ver [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


Indica si el objeto es imprimible. Si False, esta forma no se imprimirá al imprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

### setSoftEdges(double value) {#setSoftEdges-double-}
```
public void setSoftEdges(double value)
```


Establece el radio del desenfoque que se aplicará a los bordes, en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Establece el texto de esta forma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Establece la dirección del flujo de texto para este objeto.

Ver [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Establece el tipo de alineación horizontal del texto de la forma.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Establece el tipo de desbordamiento horizontal del texto de la forma que contiene texto.

Ver [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextOptions(TextOptions value) {#setTextOptions-com.aspose.cells.TextOptions-}
```
public void setTextOptions(TextOptions value)
```


Representa las opciones de texto de la forma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [TextOptions](../../com.aspose.cells/textoptions) |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


Establece el tipo de orientación del texto de la forma.

Ver [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Establece el tipo de forma de texto predefinido.

Ver [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Establece el tipo de alineación vertical del texto de la forma.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Establece el tipo de desbordamiento vertical del texto de la forma que contiene texto.

Ver [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

### setTopInShape(int value) {#setTopInShape-int-}
```
public void setTopInShape(int value)
```


Representa el desplazamiento vertical de la forma desde el borde superior de la forma padre, en unidades de 1/4000 de la altura de la forma padre.

**Remarks**

Solo se aplica cuando esta forma está en el grupo o en el gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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


Establece el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


Establece el desplazamiento horizontal de la forma desde la columna de su esquina superior izquierda.

**Remarks**

El rango de valores es de 0 a 1024.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


Establece el desplazamiento vertical de la forma desde la fila de su esquina superior izquierda.

**Remarks**

El rango de valores es de 0 a 256.

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


Representa el índice de la fila superior.

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

### setWidthInShape(int value) {#setWidthInShape-int-}
```
public void setWidthInShape(int value)
```


Representa el ancho de la forma, en unidades de 1/4000 de la forma padre.

**Remarks**

Solo se aplica cuando esta forma está en el grupo o en el gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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


Establece el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo, en unidades de píxeles.

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

### toFrontOrBack(int orders) {#toFrontOrBack-int-}
```
public void toFrontOrBack(int orders)
```


Mueve la forma al frente o la envía al fondo.

**Example**

```
         shape.toFrontOrBack(2);
         //or shape.ToFrontOrBack(-1);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| orders | int | Si es menor que cero, coloca la forma en el fondo. Si es mayor que cero, lleva la forma al frente. |

### toImage(OutputStream stream, ImageFormat imageFormat) {#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-}
```
public void toImage(OutputStream stream, ImageFormat imageFormat)
```


Crea la imagen de la forma y la guarda en un flujo en el formato especificado.

**Remarks**

Los siguientes formatos son compatibles: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo de salida. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | El formato en el que guardar la imagen. |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Guarda la forma en un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


Guarda la forma en un archivo.

**Example**

```
         ImageOrPrintOptions op = new ImageOrPrintOptions();
         shape.toImage("exmaple.png", op);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| imageFile | java.lang.String |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


Actualiza el valor seleccionado con el valor de la celda vinculada.

**Example**

```
         Cell cell = null;
         for (int i = 0; i? ++i)
         {
             cell = book.getWorksheets().get(0).getCells().get(i, 0);
             cell.setValue(i + 1);
         }
 
         //Create a ListBox object
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
 
         //Form Controls
         Shape listBox = book.getWorksheets().get(0).getShapes().addListBox(2, 0, 2, 0, 130, 130);
 
         //Sets the range used to fill the control.
         listBox.setInputRange("$A$1:$A$6", false, false);
 
         //Sets the range linked to the control's value.
         listBox.setLinkedCell("$A$12", false, true);
 
         ListBox listbx = (ListBox)listBox;
 
         //Set the value of cell A12
         cell = book.getWorksheets().get(0).getCells().get(11, 0);
         cell.setValue(3);
 
         //Update the selected value by the value of the linked cell.
         listBox.updateSelectedValue();
 
         //-1 default, no option selected
         if(listbx.isSelected(2))
         {
             //Option 3 of the ListBox is selected
         }
 
         //Change the value of a linked cell
         cell.setValue(4);
 
         //Update the selected value by the value of the linked cell.
         listBox.updateSelectedValue();
         if(listbx.isSelected(3))
         {
             //Option 4 of the ListBox is selected
         }
```

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

