---
title: "GradientFill"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il riempimento sfumato."
type: docs
url: /it/java/com.aspose.cells/gradientfill/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Fill](../../com.aspose.cells/fill)
```
public class GradientFill extends Fill
```

Rappresenta il riempimento sfumato.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | / |
| [getAngle()](#getAngle--) | L'angolo del riempimento lineare. |
| [getClass()](#getClass--) |  |
| [getDirectionType()](#getDirectionType--) | Ottiene il tipo di direzione del gradiente. |
| [getFillType()](#getFillType--) | Ottiene il tipo di riempimento del gradiente. |
| [getGradientColor1()](#getGradientColor1--) | Ottiene il colore gradiente 1. |
| [getGradientColor2()](#getGradientColor2--) | Ottiene il colore gradiente 2. |
| [getGradientColorType()](#getGradientColorType--) | Ottiene il tipo di colore gradiente. |
| [getGradientDegree()](#getGradientDegree--) | Ottiene il grado del gradiente. |
| [getGradientStops()](#getGradientStops--) | Rappresenta la raccolta di fermate del gradiente. |
| [getGradientStyle()](#getGradientStyle--) | Ottiene il tipo di stile del gradiente. |
| [getPresetColor()](#getPresetColor--) | Restituisce il colore predefinito del gradiente per il riempimento specificato. |
| [getVariant()](#getVariant--) | Ottiene la variante. |
| [hashCode()](#hashCode--) | Ottiene il codice hash. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAngle(float value)](#setAngle-float-) | L'angolo del riempimento lineare. |
| [setGradient(int type, double angle, int direction)](#setGradient-int-double-int-) | Imposta il tipo di riempimento gradiente e la direzione. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Imposta il riempimento specificato a un gradiente a un colore. |
| [setPresetColor(int value)](#setPresetColor-int-) | Restituisce il colore predefinito del gradiente per il riempimento specificato. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Imposta il riempimento specificato a una sfumatura di colore predefinito. |
| [setPresetThemeGradient(int gradientType, int themeColorType)](#setPresetThemeGradient-int-int-) | Imposta il riempimento gradiente del tema predefinito. |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Imposta il riempimento specificato a un gradiente a due colori. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Imposta il riempimento specificato a un gradiente a due colori. |
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getAngle() {#getAngle--}
```
public float getAngle()
```


L'angolo del riempimento lineare.

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


Ottiene il tipo di direzione del gradiente.

Vedi [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype).

**Returns:**
int
### getFillType() {#getFillType--}
```
public int getFillType()
```


Ottiene il tipo di riempimento del gradiente.

Vedi [GradientFillType](../../com.aspose.cells/gradientfilltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Ottiene il colore gradiente 1. Si applica a Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Ottiene il colore gradiente 2. Si applica a Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Ottiene il tipo di colore gradiente. Si applica a Excel97-2003

Vedi [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Ottiene il grado del gradiente. Si applica a Excel97-2003

**Returns:**
double
### getGradientStops() {#getGradientStops--}
```
public GradientStopCollection getGradientStops()
```


Rappresenta la raccolta di fermate del gradiente.

**Returns:**
[GradientStopCollection](../../com.aspose.cells/gradientstopcollection)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Ottiene il tipo di stile del gradiente. Si applica a Excel97-2003

Vedi [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Restituisce il colore predefinito del gradiente per il riempimento specificato. Si applica a Excel97-2003

Vedi [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getVariant() {#getVariant--}
```
public int getVariant()
```


Ottiene la variante. Si applica a Excel97-2003

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Ottiene il codice hash.

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


L'angolo del riempimento lineare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setGradient(int type, double angle, int direction) {#setGradient-int-double-int-}
```
public void setGradient(int type, double angle, int direction)
```


Imposta il tipo di riempimento gradiente e la direzione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [GradientFillType](../../com.aspose.cells/gradientfilltype). Tipo di riempimento gradiente. |
| angolo | double | L'angolo. Si applica solo per GradientFillType.Linear. |
| direction | int | [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype). Il tipo di direzione. Si applica solo per GradientFillType.Radial e GradientFillType.Rectangle. |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Imposta il riempimento specificato a un gradiente a un colore. Valido solo per Excel 2007.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Un colore di gradiente. |
| grado | double | Il grado del gradiente. Può essere un valore da 0.0 (scuro) a 1.0 (chiaro). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Stile di sfumatura del gradiente. |
| variante | int | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradiente nella finestra di dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### setPresetColor(int value) {#setPresetColor-int-}
```
public void setPresetColor(int value)
```


Restituisce il colore predefinito del gradiente per il riempimento specificato. Si applica a Excel97-2003

Vedi [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Imposta il riempimento specificato a un gradiente di colore predefinito. Si applica solo per Excel 97-2003

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Tipo di colore predefinito |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Stile di sfumatura del gradiente. |
| variante | int | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradiente nella finestra di dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### setPresetThemeGradient(int gradientType, int themeColorType) {#setPresetThemeGradient-int-int-}
```
public void setPresetThemeGradient(int gradientType, int themeColorType)
```


Imposta il riempimento gradiente del tema predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| gradientType | int | [PresetThemeGradientType](../../com.aspose.cells/presetthemegradienttype). Il tipo di gradiente predefinito. |
| themeColorType | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Il tipo di colore del tema. |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


Imposta il riempimento specificato a un gradiente a due colori. Valido solo per Excel 2007.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Un colore di gradiente. |
| color2 | [Color](../../com.aspose.cells/color) | Due colori del gradiente. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Stile di sfumatura del gradiente. |
| variante | int | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradiente nella finestra di dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


Imposta il riempimento specificato a un gradiente a due colori. Valido solo per Excel 2007.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Un colore di gradiente. |
| transparency1 | double | Il grado di trasparenza del colore1 come valore da 0,0 (opaco) a 1,0 (trasparente). |
| color2 | [Color](../../com.aspose.cells/color) | Due colori del gradiente. |
| transparency2 | double | Il grado di trasparenza del colore2 come valore da 0,0 (opaco) a 1,0 (trasparente). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Stile di sfumatura del gradiente. |
| variante | int | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradiente nella finestra di dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

