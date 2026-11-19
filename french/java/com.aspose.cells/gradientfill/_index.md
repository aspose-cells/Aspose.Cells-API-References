---
title: "GradientFill"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le remplissage en dégradé."
type: docs
url: /fr/java/com.aspose.cells/gradientfill/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Fill](../../com.aspose.cells/fill)
```
public class GradientFill extends Fill
```

Représente le remplissage en dégradé.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | / |
| [getAngle()](#getAngle--) | L'angle du remplissage linéaire. |
| [getClass()](#getClass--) |  |
| [getDirectionType()](#getDirectionType--) | Obtient le type de direction du dégradé. |
| [getFillType()](#getFillType--) | Obtient le type de remplissage du dégradé. |
| [getGradientColor1()](#getGradientColor1--) | Obtient la couleur du dégradé 1. |
| [getGradientColor2()](#getGradientColor2--) | Obtient la couleur du dégradé 2. |
| [getGradientColorType()](#getGradientColorType--) | Obtient le type de couleur du dégradé. |
| [getGradientDegree()](#getGradientDegree--) | Obtient le degré du dégradé. |
| [getGradientStops()](#getGradientStops--) | Représente la collection d'arrêts de dégradé. |
| [getGradientStyle()](#getGradientStyle--) | Obtient le type de style du dégradé. |
| [getPresetColor()](#getPresetColor--) | Renvoie la couleur prédéfinie du dégradé pour le remplissage spécifié. |
| [getVariant()](#getVariant--) | Obtient la variante. |
| [hashCode()](#hashCode--) | Obtient le code de hachage. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAngle(float value)](#setAngle-float-) | L'angle du remplissage linéaire. |
| [setGradient(int type, double angle, int direction)](#setGradient-int-double-int-) | Définissez le type de remplissage du dégradé et la direction. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Définit le remplissage spécifié à un dégradé d'une seule couleur. |
| [setPresetColor(int value)](#setPresetColor-int-) | Renvoie la couleur prédéfinie du dégradé pour le remplissage spécifié. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Définit le remplissage spécifié à un dégradé de couleur prédéfinie. |
| [setPresetThemeGradient(int gradientType, int themeColorType)](#setPresetThemeGradient-int-int-) | Définit le remplissage du dégradé de thème prédéfini. |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Définit le remplissage spécifié à un dégradé à deux couleurs. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Définit le remplissage spécifié à un dégradé à deux couleurs. |
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
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getAngle() {#getAngle--}
```
public float getAngle()
```


L'angle du remplissage linéaire.

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


Obtient le type de direction du dégradé.

Voir [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype).

**Returns:**
int
### getFillType() {#getFillType--}
```
public int getFillType()
```


Obtient le type de remplissage du dégradé.

Voir [GradientFillType](../../com.aspose.cells/gradientfilltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Obtient la couleur du dégradé 1. S'applique à Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Obtient la couleur du dégradé 2. S'applique à Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Obtient le type de couleur du dégradé. S'applique à Excel97-2003

Voir [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Obtient le degré du dégradé. S'applique à Excel97-2003

**Returns:**
double
### getGradientStops() {#getGradientStops--}
```
public GradientStopCollection getGradientStops()
```


Représente la collection d'arrêts de dégradé.

**Returns:**
[GradientStopCollection](../../com.aspose.cells/gradientstopcollection)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Obtient le type de style du dégradé. S'applique à Excel97-2003

Voir [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Renvoie la couleur prédéfinie du dégradé pour le remplissage spécifié. S'applique à Excel97-2003

Voir [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getVariant() {#getVariant--}
```
public int getVariant()
```


Obtient la variante. S'applique à Excel97-2003

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Obtient le code de hachage.

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


L'angle du remplissage linéaire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setGradient(int type, double angle, int direction) {#setGradient-int-double-int-}
```
public void setGradient(int type, double angle, int direction)
```


Définissez le type de remplissage du dégradé et la direction.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [GradientFillType](../../com.aspose.cells/gradientfilltype). Type de remplissage du dégradé. |
| angle | double | L'angle. S'applique uniquement pour GradientFillType.Linear. |
| direction | int | [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype). Le type de direction. S'applique uniquement pour GradientFillType.Radial et GradientFillType.Rectangle. |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Définit le remplissage spécifié à un dégradé à une couleur. S'applique uniquement à Excel 2007.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Une couleur de dégradé. |
| degré | double | Le degré du dégradé. Peut être une valeur de 0.0 (sombre) à 1.0 (clair). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Style d'ombrage du dégradé. |
| variante | int | La variante de dégradé. Peut être une valeur de 1 à 4, correspondant à l'une des quatre variantes dans l'onglet Gradient de la boîte de dialogue Remplissage d'effets. Si le style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2. |

### setPresetColor(int value) {#setPresetColor-int-}
```
public void setPresetColor(int value)
```


Renvoie la couleur prédéfinie du dégradé pour le remplissage spécifié. S'applique à Excel97-2003

Voir [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Définit le remplissage spécifié à un dégradé de couleur prédéfini. S'applique uniquement pour Excel 97-2003

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Type de couleur prédéfini |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Style d'ombrage du dégradé. |
| variante | int | La variante de dégradé. Peut être une valeur de 1 à 4, correspondant à l'une des quatre variantes dans l'onglet Gradient de la boîte de dialogue Remplissage d'effets. Si le style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2. |

### setPresetThemeGradient(int gradientType, int themeColorType) {#setPresetThemeGradient-int-int-}
```
public void setPresetThemeGradient(int gradientType, int themeColorType)
```


Définit le remplissage du dégradé de thème prédéfini.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| gradientType | int | [PresetThemeGradientType](../../com.aspose.cells/presetthemegradienttype). Le type de dégradé prédéfini. |
| themeColorType | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Le type de couleur du thème. |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


Définit le remplissage spécifié à un dégradé à deux couleurs. S'applique uniquement à Excel 2007.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Une couleur de dégradé. |
| color2 | [Color](../../com.aspose.cells/color) | Deux couleurs de dégradé. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Style d'ombrage du dégradé. |
| variante | int | La variante de dégradé. Peut être une valeur de 1 à 4, correspondant à l'une des quatre variantes dans l'onglet Gradient de la boîte de dialogue Remplissage d'effets. Si le style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2. |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


Définit le remplissage spécifié à un dégradé à deux couleurs. S'applique uniquement à Excel 2007.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Une couleur de dégradé. |
| transparency1 | double | Le degré de transparence de la couleur1 sous forme d'une valeur comprise entre 0.0 (opaque) et 1.0 (transparent). |
| color2 | [Color](../../com.aspose.cells/color) | Deux couleurs de dégradé. |
| transparency2 | double | Le degré de transparence de la couleur2 sous forme d'une valeur comprise entre 0.0 (opaque) et 1.0 (transparent). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Style d'ombrage du dégradé. |
| variante | int | La variante de dégradé. Peut être une valeur de 1 à 4, correspondant à l'une des quatre variantes dans l'onglet Gradient de la boîte de dialogue Remplissage d'effets. Si le style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2. |

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

