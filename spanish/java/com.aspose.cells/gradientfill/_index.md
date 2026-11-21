---
title: "GradientFill"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el relleno degradado."
type: docs
url: /es/java/com.aspose.cells/gradientfill/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Fill](../../com.aspose.cells/fill)
```
public class GradientFill extends Fill
```

Representa el relleno degradado.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | / |
| [getAngle()](#getAngle--) | El ángulo del relleno lineal. |
| [getClass()](#getClass--) |  |
| [getDirectionType()](#getDirectionType--) | Obtiene el tipo de dirección del degradado. |
| [getFillType()](#getFillType--) | Obtiene el tipo de relleno del degradado. |
| [getGradientColor1()](#getGradientColor1--) | Obtiene el color de degradado 1. |
| [getGradientColor2()](#getGradientColor2--) | Obtiene el color de degradado 2. |
| [getGradientColorType()](#getGradientColorType--) | Obtiene el tipo de color de degradado. |
| [getGradientDegree()](#getGradientDegree--) | Obtiene el grado del degradado. |
| [getGradientStops()](#getGradientStops--) | Representa la colección de paradas de degradado. |
| [getGradientStyle()](#getGradientStyle--) | Obtiene el tipo de estilo de degradado. |
| [getPresetColor()](#getPresetColor--) | Devuelve el color preestablecido del degradado para el relleno especificado. |
| [getVariant()](#getVariant--) | Obtiene la variante. |
| [hashCode()](#hashCode--) | Obtiene el código hash. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAngle(float value)](#setAngle-float-) | El ángulo del relleno lineal. |
| [setGradient(int type, double angle, int direction)](#setGradient-int-double-int-) | Establece el tipo y la dirección del relleno de degradado. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Establece el relleno especificado a un degradado de un solo color. |
| [setPresetColor(int value)](#setPresetColor-int-) | Devuelve el color preestablecido del degradado para el relleno especificado. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Establece el relleno especificado a un degradado de color preestablecido. |
| [setPresetThemeGradient(int gradientType, int themeColorType)](#setPresetThemeGradient-int-int-) | Establece el relleno de degradado de tema predefinido. |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Establece el relleno especificado a un degradado de dos colores. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Establece el relleno especificado a un degradado de dos colores. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


/

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getAngle() {#getAngle--}
```
public float getAngle()
```


El ángulo del relleno lineal.

**Returns:**
float
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


Obtiene el tipo de dirección del degradado.

Ver [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype).

**Returns:**
int
### getFillType() {#getFillType--}
```
public int getFillType()
```


Obtiene el tipo de relleno del degradado.

Ver [GradientFillType](../../com.aspose.cells/gradientfilltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Obtiene el color de degradado 1. Aplica a Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Obtiene el color de degradado 2. Aplica a Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Obtiene el tipo de color de degradado. Aplica a Excel97-2003

Ver [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Obtiene el grado del degradado. Aplica a Excel97-2003

**Returns:**
double
### getGradientStops() {#getGradientStops--}
```
public GradientStopCollection getGradientStops()
```


Representa la colección de paradas de degradado.

**Returns:**
[GradientStopCollection](../../com.aspose.cells/gradientstopcollection)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Obtiene el tipo de estilo de degradado. Aplica a Excel97-2003

Ver [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Devuelve el color predefinido del degradado para el relleno especificado. Aplica a Excel97-2003

Ver [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getVariant() {#getVariant--}
```
public int getVariant()
```


Obtiene la variante. Aplica a Excel97-2003

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Obtiene el código hash.

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




### setAngle(float value) {#setAngle-float-}
```
public void setAngle(float value)
```


El ángulo del relleno lineal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setGradient(int type, double angle, int direction) {#setGradient-int-double-int-}
```
public void setGradient(int type, double angle, int direction)
```


Establece el tipo y la dirección del relleno de degradado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [GradientFillType](../../com.aspose.cells/gradientfilltype). Tipo de relleno de degradado. |
| ángulo | double | El ángulo. Solo se aplica a GradientFillType.Linear. |
| direction | int | [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype). El tipo de dirección. Solo se aplica a GradientFillType.Radial y GradientFillType.Rectangle. |

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

### setPresetColor(int value) {#setPresetColor-int-}
```
public void setPresetColor(int value)
```


Devuelve el color predefinido del degradado para el relleno especificado. Aplica a Excel97-2003

Ver [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Establece el relleno especificado a un degradado de color predefinido. Solo se aplica a Excel 97-2003

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Tipo de color predefinido |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Estilo de sombreado del degradado. |
| variante | int | La variante de degradado. Puede ser un valor del 1 al 4, correspondiente a una de las cuatro variantes en la pestaña Degradado del cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2. |

### setPresetThemeGradient(int gradientType, int themeColorType) {#setPresetThemeGradient-int-int-}
```
public void setPresetThemeGradient(int gradientType, int themeColorType)
```


Establece el relleno de degradado de tema predefinido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| gradientType | int | [PresetThemeGradientType](../../com.aspose.cells/presetthemegradienttype). El tipo de degradado predefinido. |
| themeColorType | int | [ThemeColorType](../../com.aspose.cells/themecolortype). El tipo de color del tema. |

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

