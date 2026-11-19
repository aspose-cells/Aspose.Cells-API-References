---
title: "RenderingWatermark"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Filigrane pour le rendu."
type: docs
url: /fr/java/com.aspose.cells/renderingwatermark/
---

**Inheritance:**
java.lang.Object
```
public class RenderingWatermark
```

Filigrane pour le rendu.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [RenderingWatermark(String text, RenderingFont renderingFont)](#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-) | Crée une instance de filigrane texte. |
| [RenderingWatermark(byte[] imageData)](#RenderingWatermark-byte---) | Crée une instance de filigrane image. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Obtient la police du filigrane. |
| [getHAlignment()](#getHAlignment--) | Obtient l'alignement horizontal du filigrane par rapport à la page. |
| [getImage()](#getImage--) | Obtient l'image du filigrane. |
| [getOffsetX()](#getOffsetX--) | Obtient la valeur de décalage pour [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [getOffsetY()](#getOffsetY--) | Obtient la valeur de décalage pour [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [getOpacity()](#getOpacity--) | Obtient l'opacité du filigrane dans la plage [0, 1]. |
| [getRotation()](#getRotation--) | Obtient la rotation du filigrane en degrés. |
| [getScaleToPagePercent()](#getScaleToPagePercent--) | Obtient l'échelle relative à la page cible en pourcentage. |
| [getText()](#getText--) | Obtient le texte du filigrane. |
| [getVAlignment()](#getVAlignment--) | Obtient l'alignement vertical du filigrane par rapport à la page. |
| [hashCode()](#hashCode--) |  |
| [isBackground()](#isBackground--) | Indique si le filigrane est placé derrière le contenu de la page. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackground(boolean value)](#setBackground-boolean-) | Indique si le filigrane est placé derrière le contenu de la page. |
| [setHAlignment(int value)](#setHAlignment-int-) | Définit l'alignement horizontal du filigrane par rapport à la page. |
| [setOffsetX(float value)](#setOffsetX-float-) | Définit la valeur de décalage pour [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [setOffsetY(float value)](#setOffsetY-float-) | Définit la valeur de décalage pour [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [setOpacity(float value)](#setOpacity-float-) | Définit l'opacité du filigrane dans la plage [0, 1]. |
| [setRotation(float value)](#setRotation-float-) | Définit la rotation du filigrane en degrés. |
| [setScaleToPagePercent(int value)](#setScaleToPagePercent-int-) | Définit l'échelle relative à la page cible en pourcentage. |
| [setVAlignment(int value)](#setVAlignment-int-) | Définit l'alignement vertical du filigrane par rapport à la page. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### RenderingWatermark(String text, RenderingFont renderingFont) {#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-}
```
public RenderingWatermark(String text, RenderingFont renderingFont)
```


Crée une instance de filigrane texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| texte | java.lang.String | texte du filigrane |
| renderingFont | [RenderingFont](../../com.aspose.cells/renderingfont) | police du filigrane |

### RenderingWatermark(byte[] imageData) {#RenderingWatermark-byte---}
```
public RenderingWatermark(byte[] imageData)
```


Crée une instance de filigrane image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| imageData | byte[] |  |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public RenderingFont getFont()
```


Obtient la police du filigrane.

**Returns:**
[RenderingFont](../../com.aspose.cells/renderingfont)
### getHAlignment() {#getHAlignment--}
```
public int getHAlignment()
```


Obtient l'alignement horizontal du filigrane par rapport à la page.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Seuls Left, Center, Right sont valides. La valeur par défaut est Left.

**Returns:**
int
### getImage() {#getImage--}
```
public byte[] getImage()
```


Obtient l'image du filigrane.

**Returns:**
byte[]
### getOffsetX() {#getOffsetX--}
```
public float getOffsetX()
```


Obtient la valeur de décalage pour [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Returns:**
float
### getOffsetY() {#getOffsetY--}
```
public float getOffsetY()
```


Obtient la valeur de décalage pour [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Returns:**
float
### getOpacity() {#getOpacity--}
```
public float getOpacity()
```


Obtient l'opacité du filigrane dans la plage [0, 1].

**Returns:**
float
### getRotation() {#getRotation--}
```
public float getRotation()
```


Obtient la rotation du filigrane en degrés.

**Returns:**
float
### getScaleToPagePercent() {#getScaleToPagePercent--}
```
public int getScaleToPagePercent()
```


Obtient l'échelle relative à la page cible en pourcentage.

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Obtient le texte du filigrane.

**Returns:**
java.lang.String
### getVAlignment() {#getVAlignment--}
```
public int getVAlignment()
```


Obtient l'alignement vertical du filigrane par rapport à la page.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Seuls Top, Center, Bottom sont valides. La valeur par défaut est Top.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBackground() {#isBackground--}
```
public boolean isBackground()
```


Indique si le filigrane est placé derrière le contenu de la page.

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




### setBackground(boolean value) {#setBackground-boolean-}
```
public void setBackground(boolean value)
```


Indique si le filigrane est placé derrière le contenu de la page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHAlignment(int value) {#setHAlignment-int-}
```
public void setHAlignment(int value)
```


Définit l'alignement horizontal du filigrane par rapport à la page.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Seuls Left, Center, Right sont valides. La valeur par défaut est Left.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setOffsetX(float value) {#setOffsetX-float-}
```
public void setOffsetX(float value)
```


Définit la valeur de décalage pour [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setOffsetY(float value) {#setOffsetY-float-}
```
public void setOffsetY(float value)
```


Définit la valeur de décalage pour [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setOpacity(float value) {#setOpacity-float-}
```
public void setOpacity(float value)
```


Définit l'opacité du filigrane dans la plage [0, 1].

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setRotation(float value) {#setRotation-float-}
```
public void setRotation(float value)
```


Définit la rotation du filigrane en degrés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setScaleToPagePercent(int value) {#setScaleToPagePercent-int-}
```
public void setScaleToPagePercent(int value)
```


Définit l'échelle relative à la page cible en pourcentage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setVAlignment(int value) {#setVAlignment-int-}
```
public void setVAlignment(int value)
```


Définit l'alignement vertical du filigrane par rapport à la page.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Seuls Top, Center, Bottom sont valides. La valeur par défaut est Top.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

