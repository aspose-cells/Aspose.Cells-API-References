---
title: "LineFormat"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa todas las configuraciones de la línea."
type: docs
url: /es/java/com.aspose.cells/lineformat/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FillFormat](../../com.aspose.cells/fillformat)
```
public class LineFormat extends FillFormat
```

Representa todas las configuraciones de la línea.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
         Shape shape = shapes.addRectangle(1, 0, 1, 0, 50, 100);
         LineFormat lineFmt = shape.getLine();
 
         //do your business
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina si esta instancia tiene el mismo valor que otro objeto [LineFormat](../../com.aspose.cells/lineformat) especificado. |
| [getBeginArrowheadLength()](#getBeginArrowheadLength--) | Obtiene el tipo de longitud de la flecha inicial de la línea. |
| [getBeginArrowheadStyle()](#getBeginArrowheadStyle--) | Obtiene el tipo de flecha inicial de la línea. |
| [getBeginArrowheadWidth()](#getBeginArrowheadWidth--) | Obtiene el tipo de ancho de la flecha inicial de la línea. |
| [getCapType()](#getCapType--) | Especifica los extremos finales. |
| [getClass()](#getClass--) |  |
| [getCompoundType()](#getCompoundType--) | Especifica el tipo compuesto de la línea. |
| [getDashStyle()](#getDashStyle--) | Especifica el tipo de guión de la línea. |
| [getEndArrowheadLength()](#getEndArrowheadLength--) | Obtiene el tipo de longitud de la flecha final de la línea. |
| [getEndArrowheadStyle()](#getEndArrowheadStyle--) | Obtiene el tipo de flecha final de la línea. |
| [getEndArrowheadWidth()](#getEndArrowheadWidth--) | Obtiene el tipo de ancho de la flecha final de la línea. |
| [getFillType()](#getFillType--) | Obtiene el tipo de relleno |
| [getGradientColor1()](#getGradientColor1--) | Devuelve el color de degradado 1 para el relleno especificado. |
| [getGradientColor2()](#getGradientColor2--) | Devuelve el color de degradado 2 para el relleno especificado. |
| [getGradientColorType()](#getGradientColorType--) | Devuelve el tipo de color de degradado para el relleno especificado. |
| [getGradientDegree()](#getGradientDegree--) | Devuelve el grado del degradado para el relleno especificado. |
| [getGradientFill()](#getGradientFill--) | Obtiene el objeto [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--). |
| [getGradientStyle()](#getGradientStyle--) | Devuelve el estilo del degradado para el relleno especificado. |
| [getGradientVariant()](#getGradientVariant--) | Devuelve la variante del degradado para el relleno especificado. |
| [getImageData()](#getImageData--) | Obtiene los datos de la imagen. |
| [getJoinType()](#getJoinType--) | Especifica el tipo de unión de la línea. |
| [getPattern()](#getPattern--) | Representa el patrón de visualización de un área. |
| [getPatternFill()](#getPatternFill--) | Obtiene el objeto [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--). |
| [getPictureFormatType()](#getPictureFormatType--) | Obtiene el tipo de formato de imagen. |
| [getPresetColor()](#getPresetColor--) | Devuelve el color preestablecido del degradado para el relleno especificado. |
| [getScale()](#getScale--) | Obtiene la escala del formato de imagen. |
| [getSetType()](#getSetType--) | Obtiene el tipo de conjunto de formato de relleno. |
| [getSolidFill()](#getSolidFill--) | Obtiene el objeto [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--). |
| [getTexture()](#getTexture--) | Representa el tipo de textura para el relleno especificado. |
| [getTextureFill()](#getTextureFill--) | Obtiene el objeto [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--). |
| [getTransparency()](#getTransparency--) | Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (transparente). |
| [getType()](#getType--) | Obtiene el tipo de relleno. |
| [getWeight()](#getWeight--) | Obtiene el grosor de la línea en unidades de puntos. |
| [hashCode()](#hashCode--) | Obtiene el código hash. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBeginArrowheadLength(int value)](#setBeginArrowheadLength-int-) | Establece el tipo de longitud de la flecha inicial de la línea. |
| [setBeginArrowheadStyle(int value)](#setBeginArrowheadStyle-int-) | Establece el tipo de flecha inicial de la línea. |
| [setBeginArrowheadWidth(int value)](#setBeginArrowheadWidth-int-) | Establece el tipo de ancho de la flecha inicial de la línea. |
| [setCapType(int value)](#setCapType-int-) | Especifica los extremos finales. |
| [setCompoundType(int value)](#setCompoundType-int-) | Especifica el tipo compuesto de la línea. |
| [setDashStyle(int value)](#setDashStyle-int-) | Especifica el tipo de guión de la línea. |
| [setEndArrowheadLength(int value)](#setEndArrowheadLength-int-) | Establece el tipo de longitud de la flecha final de la línea. |
| [setEndArrowheadStyle(int value)](#setEndArrowheadStyle-int-) | Establece el tipo de flecha final de la línea. |
| [setEndArrowheadWidth(int value)](#setEndArrowheadWidth-int-) | Establece el tipo de ancho de la flecha final de la línea. |
| [setFillType(int value)](#setFillType-int-) | Establece el tipo de relleno |
| [setImageData(byte[] value)](#setImageData-byte---) | Establece los datos de la imagen. |
| [setJoinType(int value)](#setJoinType-int-) | Especifica el tipo de unión de la línea. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Establece el relleno especificado a un degradado de un solo color. |
| [setPattern(int value)](#setPattern-int-) | Representa el patrón de visualización de un área. |
| [setPictureFormatType(int value)](#setPictureFormatType-int-) | Establece el tipo de formato de imagen. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Establece el relleno especificado a un degradado de color preestablecido. |
| [setScale(double value)](#setScale-double-) | Establece la escala del formato de imagen. |
| [setSetType(int value)](#setSetType-int-) | Obtiene el tipo de conjunto de formato de relleno. |
| [setTexture(int value)](#setTexture-int-) | Representa el tipo de textura para el relleno especificado. |
| [setTransparency(double value)](#setTransparency-double-) | Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (transparente). |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Establece el relleno especificado a un degradado de dos colores. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Establece el relleno especificado a un degradado de dos colores. |
| [setType(int value)](#setType-int-) | Establece el tipo de relleno. |
| [setWeight(double value)](#setWeight-double-) | Establece el peso de la línea en unidades de puntos. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determina si esta instancia tiene el mismo valor que otro objeto [LineFormat](../../com.aspose.cells/lineformat) especificado.

**Example**

```
         //You have to make sure that the index value in this line of code exists
         LineFormat obj = workbook.getWorksheets().get(0).getShapes().get(0).getLine();
         if (lineFmt.equals(obj))
         {
             //do what you want
         }
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | El objeto [LineFormat](../../com.aspose.cells/lineformat) para comparar con esta instancia. |

**Returns:**
boolean - true si el valor del parámetro obj es el mismo que el valor de esta instancia; de lo contrario, false. Si obj es null, este método devuelve false.
### getBeginArrowheadLength() {#getBeginArrowheadLength--}
```
public int getBeginArrowheadLength()
```


Obtiene el tipo de longitud de la flecha inicial de la línea.

Ver [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Example**

```
         lineFmt.setBeginArrowheadLength(MsoArrowheadLength.LONG);
```

**Returns:**
int
### getBeginArrowheadStyle() {#getBeginArrowheadStyle--}
```
public int getBeginArrowheadStyle()
```


Obtiene el tipo de flecha inicial de la línea.

Ver [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Example**

```
         lineFmt.setBeginArrowheadStyle(MsoArrowheadStyle.ARROW_OPEN);
```

**Returns:**
int
### getBeginArrowheadWidth() {#getBeginArrowheadWidth--}
```
public int getBeginArrowheadWidth()
```


Obtiene el tipo de ancho de la flecha inicial de la línea.

Ver [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Example**

```
         lineFmt.setBeginArrowheadWidth(MsoArrowheadWidth.MEDIUM);
```

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


Especifica los extremos finales.

Ver [LineCapType](../../com.aspose.cells/linecaptype).

**Example**

```
         lineFmt.setCapType(LineCapType.FLAT);
```

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


Especifica el tipo compuesto de la línea.

Ver [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Example**

```
         lineFmt.setCompoundType(MsoLineStyle.SINGLE);
```

**Returns:**
int
### getDashStyle() {#getDashStyle--}
```
public int getDashStyle()
```


Especifica el tipo de guión de la línea.

Ver [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Example**

```
         lineFmt.setDashStyle(MsoLineDashStyle.SOLID);
```

**Returns:**
int
### getEndArrowheadLength() {#getEndArrowheadLength--}
```
public int getEndArrowheadLength()
```


Obtiene el tipo de longitud de la flecha final de la línea.

Ver [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Example**

```
         lineFmt.setEndArrowheadLength(MsoArrowheadLength.LONG);
```

**Returns:**
int
### getEndArrowheadStyle() {#getEndArrowheadStyle--}
```
public int getEndArrowheadStyle()
```


Obtiene el tipo de flecha final de la línea.

Ver [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Example**

```
         lineFmt.setEndArrowheadStyle(MsoArrowheadStyle.ARROW_OPEN);
```

**Returns:**
int
### getEndArrowheadWidth() {#getEndArrowheadWidth--}
```
public int getEndArrowheadWidth()
```


Obtiene el tipo de ancho de la flecha final de la línea.

Ver [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Example**

```
         lineFmt.setEndArrowheadWidth(MsoArrowheadWidth.MEDIUM);
```

**Returns:**
int
### getFillType() {#getFillType--}
```
public int getFillType()
```


Obtiene el tipo de relleno

Ver [FillType](../../com.aspose.cells/filltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Devuelve el color de degradado 1 para el relleno especificado.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Devuelve el color de degradado 2 para el relleno especificado.

**Remarks**

Solo cuando el tipo de color del degradado es GradientColorType.TwoColors, esta propiedad tiene sentido.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Devuelve el tipo de color de degradado para el relleno especificado.

Ver [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Devuelve el grado del degradado para el relleno especificado. Solo se aplica a Excel 2007.

**Remarks**

Solo puede ser un valor entre 0.0 (oscuro) y 1.0 (claro).

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Obtiene el objeto [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--).

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Devuelve el estilo del degradado para el relleno especificado.

Ver [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getGradientVariant() {#getGradientVariant--}
```
public int getGradientVariant()
```


Devuelve la variante del degradado para el relleno especificado. Solo se aplica a Excel 2007.

**Remarks**

Solo puede ser un valor entre 1 y 4, correspondiente a una de las cuatro variantes en la pestaña Degradado del cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2.

**Returns:**
int
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Obtiene los datos de la imagen.

**Remarks**

Si el formato de relleno no es un formato de textura personalizada, devuelve null.

**Returns:**
byte[]
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Especifica el tipo de unión de la línea.

Ver [LineJoinType](../../com.aspose.cells/linejointype).

**Example**

```
         lineFmt.setJoinType(LineJoinType.ROUND);
```

**Returns:**
int
### getPattern() {#getPattern--}
```
public int getPattern()
```


Representa el patrón de visualización de un área.

Ver [FillPattern](../../com.aspose.cells/fillpattern).

**Returns:**
int
### getPatternFill() {#getPatternFill--}
```
public PatternFill getPatternFill()
```


Obtiene el objeto [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--).

**Returns:**
[PatternFill](../../com.aspose.cells/patternfill)
### getPictureFormatType() {#getPictureFormatType--}
```
public int getPictureFormatType()
```


Obtiene el tipo de formato de imagen.

Ver [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Devuelve el color preestablecido del degradado para el relleno especificado.

Ver [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getScale() {#getScale--}
```
public double getScale()
```


Obtiene la escala del formato de imagen.

**Returns:**
double
### getSetType() {#getSetType--}
```
public int getSetType()
```


Obtiene el tipo de conjunto de formato de relleno.

Ver [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad FillFormat.FillType. Esta propiedad será eliminada 12 meses después desde julio de 2016. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getSolidFill() {#getSolidFill--}
```
public SolidFill getSolidFill()
```


Obtiene el objeto [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--).

**Returns:**
[SolidFill](../../com.aspose.cells/solidfill)
### getTexture() {#getTexture--}
```
public int getTexture()
```


Representa el tipo de textura para el relleno especificado.

Ver [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
### getTextureFill() {#getTextureFill--}
```
public TextureFill getTextureFill()
```


Obtiene el objeto [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--).

**Returns:**
[TextureFill](../../com.aspose.cells/texturefill)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (transparente).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Obtiene el tipo de relleno.

Ver [FillType](../../com.aspose.cells/filltype).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad FillFormat.FillType. Esta propiedad será eliminada 12 meses después desde julio de 2016. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getWeight() {#getWeight--}
```
public double getWeight()
```


Obtiene el grosor de la línea en unidades de puntos.

**Example**

```
         lineFmt.setWeight(2.0d);
```

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```


Obtiene el código hash.

**Example**

```
         int hashCode = lineFmt.hashCode();
```

**Returns:**
int -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBeginArrowheadLength(int value) {#setBeginArrowheadLength-int-}
```
public void setBeginArrowheadLength(int value)
```


Establece el tipo de longitud de la flecha inicial de la línea.

Ver [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBeginArrowheadStyle(int value) {#setBeginArrowheadStyle-int-}
```
public void setBeginArrowheadStyle(int value)
```


Establece el tipo de flecha inicial de la línea.

Ver [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBeginArrowheadWidth(int value) {#setBeginArrowheadWidth-int-}
```
public void setBeginArrowheadWidth(int value)
```


Establece el tipo de ancho de la flecha inicial de la línea.

Ver [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


Especifica los extremos finales.

Ver [LineCapType](../../com.aspose.cells/linecaptype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


Especifica el tipo compuesto de la línea.

Ver [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDashStyle(int value) {#setDashStyle-int-}
```
public void setDashStyle(int value)
```


Especifica el tipo de guión de la línea.

Ver [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setEndArrowheadLength(int value) {#setEndArrowheadLength-int-}
```
public void setEndArrowheadLength(int value)
```


Establece el tipo de longitud de la flecha final de la línea.

Ver [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setEndArrowheadStyle(int value) {#setEndArrowheadStyle-int-}
```
public void setEndArrowheadStyle(int value)
```


Establece el tipo de flecha final de la línea.

Ver [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setEndArrowheadWidth(int value) {#setEndArrowheadWidth-int-}
```
public void setEndArrowheadWidth(int value)
```


Establece el tipo de ancho de la flecha final de la línea.

Ver [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setFillType(int value) {#setFillType-int-}
```
public void setFillType(int value)
```


Establece el tipo de relleno

Ver [FillType](../../com.aspose.cells/filltype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


Establece los datos de la imagen.

**Remarks**

Si el formato de relleno no es un formato de textura personalizada, devuelve null.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte[] |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


Especifica el tipo de unión de la línea.

Ver [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Establece el relleno especificado a un degradado de un color. Solo se aplica a Excel 2007.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Un color de degradado. |
| grado | double | El grado del degradado. Puede ser un valor de 0.0 (oscuro) a 1.0 (claro). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Estilo de sombreado del degradado. |
| variante | int | La variante de degradado. Puede ser un valor del 1 al 4, correspondiente a una de las cuatro variantes en la pestaña Degradado del cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2. |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


Representa el patrón de visualización de un área.

Ver [FillPattern](../../com.aspose.cells/fillpattern).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPictureFormatType(int value) {#setPictureFormatType-int-}
```
public void setPictureFormatType(int value)
```


Establece el tipo de formato de imagen.

Ver [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Establece el relleno especificado a un degradado de color predefinido. Solo se aplica a Excel 2007.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Tipo de color predefinido |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Estilo de sombreado del degradado. |
| variante | int | La variante de degradado. Puede ser un valor del 1 al 4, correspondiente a una de las cuatro variantes en la pestaña Degradado del cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2. |

### setScale(double value) {#setScale-double-}
```
public void setScale(double value)
```


Establece la escala del formato de imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setSetType(int value) {#setSetType-int-}
```
public void setSetType(int value)
```


Obtiene el tipo de conjunto de formato de relleno.

Ver [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad FillFormat.FillType. Esta propiedad será eliminada 12 meses después desde julio de 2016. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTexture(int value) {#setTexture-int-}
```
public void setTexture(int value)
```


Representa el tipo de textura para el relleno especificado.

Ver [TextureType](../../com.aspose.cells/texturetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (transparente).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


Establece el relleno especificado a un degradado de dos colores. Solo se aplica a Excel 2007.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Un color de degradado. |
| color2 | [Color](../../com.aspose.cells/color) | Dos colores de degradado. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Estilo de sombreado del degradado. |
| variante | int | La variante de degradado. Puede ser un valor del 1 al 4, correspondiente a una de las cuatro variantes en la pestaña Degradado del cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2. |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


Establece el relleno especificado a un degradado de dos colores. Solo se aplica a Excel 2007.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Un color de degradado. |
| transparency1 | double | El grado de transparencia del color1 como un valor entre 0.0 (opaco) y 1.0 (transparente). |
| color2 | [Color](../../com.aspose.cells/color) | Dos colores de degradado. |
| transparency2 | double | El grado de transparencia del color2 como un valor entre 0.0 (opaco) y 1.0 (transparente). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Estilo de sombreado del degradado. |
| variante | int | La variante de degradado. Puede ser un valor del 1 al 4, correspondiente a una de las cuatro variantes en la pestaña Degradado del cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2. |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Establece el tipo de relleno.

Ver [FillType](../../com.aspose.cells/filltype).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad FillFormat.FillType. Esta propiedad será eliminada 12 meses después desde julio de 2016. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setWeight(double value) {#setWeight-double-}
```
public void setWeight(double value)
```


Establece el peso de la línea en unidades de puntos.

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

