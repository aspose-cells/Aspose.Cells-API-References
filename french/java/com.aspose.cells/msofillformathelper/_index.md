---
title: "MsoFillFormatHelper"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le format de remplissage d'une forme."
type: docs
url: /fr/java/com.aspose.cells/msofillformathelper/
---

**Inheritance:**
java.lang.Object
```
public class MsoFillFormatHelper
```

Représente le format de remplissage d'une forme.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | Obtient la couleur de fond du fichier. |
| [getClass()](#getClass--) |  |
| [getForeColor()](#getForeColor--) | Obtient la couleur de premier plan du remplissage. |
| [getForeColorTransparency()](#getForeColorTransparency--) | Renvoie ou définit le degré de couleur de premier plan du remplissage spécifié comme une valeur de 0.0 (opaque) à 1.0 (transparent). |
| [getImageData()](#getImageData--) | Obtient les données de remplissage Texture et Image. |
| [getTexture()](#getTexture--) | Obtient le type de remplissage de texture. |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | Indique s'il y a un remplissage. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.cells.Color-) | Définit la couleur de fond du fichier. |
| [setForeColor(Color value)](#setForeColor-com.aspose.cells.Color-) | Définit la couleur de premier plan du remplissage. |
| [setForeColorTransparency(double value)](#setForeColorTransparency-double-) | Renvoie ou définit le degré de couleur de premier plan du remplissage spécifié comme une valeur de 0.0 (opaque) à 1.0 (transparent). |
| [setImageData(byte[] value)](#setImageData-byte---) | Définit les données de remplissage Texture et Image. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Définit le remplissage spécifié à un dégradé d'une seule couleur. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indique s'il y a un remplissage. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Obtient la couleur de fond du fichier.

**Returns:**
[Color](../../com.aspose.cells/color)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Obtient la couleur de premier plan du remplissage.

**Returns:**
[Color](../../com.aspose.cells/color)
### getForeColorTransparency() {#getForeColorTransparency--}
```
public double getForeColorTransparency()
```


Renvoie ou définit le degré de couleur de premier plan du remplissage spécifié comme une valeur de 0.0 (opaque) à 1.0 (transparent).

**Returns:**
double
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Obtient les données de remplissage Texture et Image.

**Returns:**
byte[]
### getTexture() {#getTexture--}
```
public int getTexture()
```


Obtient le type de remplissage de texture.

Voir [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Indique s'il y a un remplissage.

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




### setBackColor(Color value) {#setBackColor-com.aspose.cells.Color-}
```
public void setBackColor(Color value)
```


Définit la couleur de fond du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColor(Color value) {#setForeColor-com.aspose.cells.Color-}
```
public void setForeColor(Color value)
```


Définit la couleur de premier plan du remplissage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColorTransparency(double value) {#setForeColorTransparency-double-}
```
public void setForeColorTransparency(double value)
```


Renvoie ou définit le degré de couleur de premier plan du remplissage spécifié comme une valeur de 0.0 (opaque) à 1.0 (transparent).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


Définit les données de remplissage Texture et Image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte[] |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Définit le remplissage spécifié à un dégradé d'une seule couleur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Une couleur de dégradé. |
| degré | double | Le degré du dégradé. Peut être une valeur de 0.0 (sombre) à 1.0 (clair). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Style d'ombrage du dégradé. |
| variante | int | La variante de dégradé. Peut être une valeur de 1 à 4, correspondant à l'une des quatre variantes dans l'onglet Gradient de la boîte de dialogue Remplissage d'effets. Si le style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2. |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indique s'il y a un remplissage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

