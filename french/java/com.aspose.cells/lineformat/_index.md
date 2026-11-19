---
title: "LineFormat"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente tous les paramètres de la ligne."
type: docs
url: /fr/java/com.aspose.cells/lineformat/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FillFormat](../../com.aspose.cells/fillformat)
```
public class LineFormat extends FillFormat
```

Représente tous les paramètres de la ligne.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
         Shape shape = shapes.addRectangle(1, 0, 1, 0, 50, 100);
         LineFormat lineFmt = shape.getLine();
 
         //do your business
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Détermine si cette instance a la même valeur qu'un autre objet [LineFormat](../../com.aspose.cells/lineformat) spécifié. |
| [getBeginArrowheadLength()](#getBeginArrowheadLength--) | Obtient le type de longueur de la flèche de début de la ligne. |
| [getBeginArrowheadStyle()](#getBeginArrowheadStyle--) | Obtient le type de flèche de début de la ligne. |
| [getBeginArrowheadWidth()](#getBeginArrowheadWidth--) | Obtient le type de largeur de la flèche de début de la ligne. |
| [getCapType()](#getCapType--) | Spécifie les embouts de fin. |
| [getClass()](#getClass--) |  |
| [getCompoundType()](#getCompoundType--) | Spécifie le type de composition de la ligne. |
| [getDashStyle()](#getDashStyle--) | Spécifie le type de tiret de la ligne. |
| [getEndArrowheadLength()](#getEndArrowheadLength--) | Obtient le type de longueur de la flèche de fin de la ligne. |
| [getEndArrowheadStyle()](#getEndArrowheadStyle--) | Obtient le type de flèche de fin de la ligne. |
| [getEndArrowheadWidth()](#getEndArrowheadWidth--) | Obtient le type de largeur de la flèche de fin de la ligne. |
| [getFillType()](#getFillType--) | Obtient le type de remplissage |
| [getGradientColor1()](#getGradientColor1--) | Renvoie la couleur de dégradé 1 pour le remplissage spécifié. |
| [getGradientColor2()](#getGradientColor2--) | Renvoie la couleur de dégradé 2 pour le remplissage spécifié. |
| [getGradientColorType()](#getGradientColorType--) | Renvoie le type de couleur de dégradé pour le remplissage spécifié. |
| [getGradientDegree()](#getGradientDegree--) | Renvoie le degré du dégradé pour le remplissage spécifié. |
| [getGradientFill()](#getGradientFill--) | Obtient l'objet [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--). |
| [getGradientStyle()](#getGradientStyle--) | Renvoie le style du dégradé pour le remplissage spécifié. |
| [getGradientVariant()](#getGradientVariant--) | Renvoie la variante du dégradé pour le remplissage spécifié. |
| [getImageData()](#getImageData--) | Obtient les données d'image de la picture. |
| [getJoinType()](#getJoinType--) | Spécifie le type de jointure de la ligne. |
| [getPattern()](#getPattern--) | Représente le motif d'affichage d'une zone. |
| [getPatternFill()](#getPatternFill--) | Obtient l'objet [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--). |
| [getPictureFormatType()](#getPictureFormatType--) | Obtient le type de format d'image. |
| [getPresetColor()](#getPresetColor--) | Renvoie la couleur prédéfinie du dégradé pour le remplissage spécifié. |
| [getScale()](#getScale--) | Obtient l'échelle du format d'image. |
| [getSetType()](#getSetType--) | Obtient le type du jeu de format de remplissage. |
| [getSolidFill()](#getSolidFill--) | Obtient l'objet [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--). |
| [getTexture()](#getTexture--) | Représente le type de texture pour le remplissage spécifié. |
| [getTextureFill()](#getTextureFill--) | Obtient l'objet [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--). |
| [getTransparency()](#getTransparency--) | Renvoie ou définit le degré de transparence de la zone sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent). |
| [getType()](#getType--) | Obtient le type de remplissage. |
| [getWeight()](#getWeight--) | Obtient le poids de la ligne en unité de points. |
| [hashCode()](#hashCode--) | Obtient le code de hachage. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBeginArrowheadLength(int value)](#setBeginArrowheadLength-int-) | Définit le type de longueur de la flèche de début de la ligne. |
| [setBeginArrowheadStyle(int value)](#setBeginArrowheadStyle-int-) | Définit le type de flèche de début de la ligne. |
| [setBeginArrowheadWidth(int value)](#setBeginArrowheadWidth-int-) | Définit le type de largeur de la flèche de début de la ligne. |
| [setCapType(int value)](#setCapType-int-) | Spécifie les embouts de fin. |
| [setCompoundType(int value)](#setCompoundType-int-) | Spécifie le type de composition de la ligne. |
| [setDashStyle(int value)](#setDashStyle-int-) | Spécifie le type de tiret de la ligne. |
| [setEndArrowheadLength(int value)](#setEndArrowheadLength-int-) | Définit le type de longueur de la flèche finale de la ligne. |
| [setEndArrowheadStyle(int value)](#setEndArrowheadStyle-int-) | Définit le type de flèche finale de la ligne. |
| [setEndArrowheadWidth(int value)](#setEndArrowheadWidth-int-) | Définit le type de largeur de la flèche finale de la ligne. |
| [setFillType(int value)](#setFillType-int-) | Définit le type de remplissage |
| [setImageData(byte[] value)](#setImageData-byte---) | Définit les données d'image de la picture. |
| [setJoinType(int value)](#setJoinType-int-) | Spécifie le type de jointure de la ligne. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Définit le remplissage spécifié à un dégradé d'une seule couleur. |
| [setPattern(int value)](#setPattern-int-) | Représente le motif d'affichage d'une zone. |
| [setPictureFormatType(int value)](#setPictureFormatType-int-) | Définit le type de format d'image. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Définit le remplissage spécifié à un dégradé de couleur prédéfinie. |
| [setScale(double value)](#setScale-double-) | Définit l'échelle du format d'image. |
| [setSetType(int value)](#setSetType-int-) | Obtient le type du jeu de format de remplissage. |
| [setTexture(int value)](#setTexture-int-) | Représente le type de texture pour le remplissage spécifié. |
| [setTransparency(double value)](#setTransparency-double-) | Renvoie ou définit le degré de transparence de la zone sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent). |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Définit le remplissage spécifié à un dégradé à deux couleurs. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Définit le remplissage spécifié à un dégradé à deux couleurs. |
| [setType(int value)](#setType-int-) | Définit le type de remplissage. |
| [setWeight(double value)](#setWeight-double-) | Définit le poids de la ligne en unité de points. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Détermine si cette instance a la même valeur qu'un autre objet [LineFormat](../../com.aspose.cells/lineformat) spécifié.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | L'objet [LineFormat](../../com.aspose.cells/lineformat) à comparer avec cette instance. |

**Returns:**
booléen - true si la valeur du paramètre obj est la même que la valeur de cette instance ; sinon, false. Si obj est null, cette méthode renvoie false.
### getBeginArrowheadLength() {#getBeginArrowheadLength--}
```
public int getBeginArrowheadLength()
```


Obtient le type de longueur de la flèche de début de la ligne.

Voir [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

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


Obtient le type de flèche de début de la ligne.

Voir [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

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


Obtient le type de largeur de la flèche de début de la ligne.

Voir [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

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


Spécifie les embouts de fin.

Voir [LineCapType](../../com.aspose.cells/linecaptype).

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


Spécifie le type de composition de la ligne.

Voir [MsoLineStyle](../../com.aspose.cells/msolinestyle).

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


Spécifie le type de tiret de la ligne.

Voir [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

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


Obtient le type de longueur de la flèche de fin de la ligne.

Voir [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

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


Obtient le type de flèche de fin de la ligne.

Voir [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

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


Obtient le type de largeur de la flèche de fin de la ligne.

Voir [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

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


Obtient le type de remplissage

Voir [FillType](../../com.aspose.cells/filltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Renvoie la couleur de dégradé 1 pour le remplissage spécifié.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Renvoie la couleur de dégradé 2 pour le remplissage spécifié.

**Remarks**

Uniquement lorsque le type de couleur du dégradé est GradientColorType.TwoColors, cette propriété a un sens.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Renvoie le type de couleur de dégradé pour le remplissage spécifié.

Voir [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Renvoie le degré du dégradé pour le remplissage spécifié. S'applique uniquement à Excel 2007.

**Remarks**

Ne peut être qu'une valeur comprise entre 0.0 (sombre) et 1.0 (clair).

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Obtient l'objet [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--).

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Renvoie le style du dégradé pour le remplissage spécifié.

Voir [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getGradientVariant() {#getGradientVariant--}
```
public int getGradientVariant()
```


Renvoie la variante du dégradé pour le remplissage spécifié. S'applique uniquement à Excel 2007.

**Remarks**

Ne peut être qu'une valeur comprise entre 1 et 4, correspondant à l'une des quatre variantes dans l'onglet Gradient de la boîte de dialogue Effets de remplissage. Si le style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2.

**Returns:**
int
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Obtient les données d'image de la picture.

**Remarks**

Si le format de remplissage n'est pas un format de texture personnalisé, renvoie null.

**Returns:**
byte[]
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Spécifie le type de jointure de la ligne.

Voir [LineJoinType](../../com.aspose.cells/linejointype).

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


Représente le motif d'affichage d'une zone.

Voir [FillPattern](../../com.aspose.cells/fillpattern).

**Returns:**
int
### getPatternFill() {#getPatternFill--}
```
public PatternFill getPatternFill()
```


Obtient l'objet [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--).

**Returns:**
[PatternFill](../../com.aspose.cells/patternfill)
### getPictureFormatType() {#getPictureFormatType--}
```
public int getPictureFormatType()
```


Obtient le type de format d'image.

Voir [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Renvoie la couleur prédéfinie du dégradé pour le remplissage spécifié.

Voir [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getScale() {#getScale--}
```
public double getScale()
```


Obtient l'échelle du format d'image.

**Returns:**
double
### getSetType() {#getSetType--}
```
public int getSetType()
```


Obtient le type du jeu de format de remplissage.

Voir [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété FillFormat.FillType. Cette propriété sera supprimée 12 mois plus tard, depuis juillet 2016. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getSolidFill() {#getSolidFill--}
```
public SolidFill getSolidFill()
```


Obtient l'objet [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--).

**Returns:**
[SolidFill](../../com.aspose.cells/solidfill)
### getTexture() {#getTexture--}
```
public int getTexture()
```


Représente le type de texture pour le remplissage spécifié.

Voir [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
### getTextureFill() {#getTextureFill--}
```
public TextureFill getTextureFill()
```


Obtient l'objet [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--).

**Returns:**
[TextureFill](../../com.aspose.cells/texturefill)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Renvoie ou définit le degré de transparence de la zone sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Obtient le type de remplissage.

Voir [FillType](../../com.aspose.cells/filltype).

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété FillFormat.FillType. Cette propriété sera supprimée 12 mois plus tard, depuis juillet 2016. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getWeight() {#getWeight--}
```
public double getWeight()
```


Obtient le poids de la ligne en unité de points.

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


Obtient le code de hachage.

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


Définit le type de longueur de la flèche de début de la ligne.

Voir [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBeginArrowheadStyle(int value) {#setBeginArrowheadStyle-int-}
```
public void setBeginArrowheadStyle(int value)
```


Définit le type de flèche de début de la ligne.

Voir [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBeginArrowheadWidth(int value) {#setBeginArrowheadWidth-int-}
```
public void setBeginArrowheadWidth(int value)
```


Définit le type de largeur de la flèche de début de la ligne.

Voir [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


Spécifie les embouts de fin.

Voir [LineCapType](../../com.aspose.cells/linecaptype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


Spécifie le type de composition de la ligne.

Voir [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDashStyle(int value) {#setDashStyle-int-}
```
public void setDashStyle(int value)
```


Spécifie le type de tiret de la ligne.

Voir [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setEndArrowheadLength(int value) {#setEndArrowheadLength-int-}
```
public void setEndArrowheadLength(int value)
```


Définit le type de longueur de la flèche finale de la ligne.

Voir [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setEndArrowheadStyle(int value) {#setEndArrowheadStyle-int-}
```
public void setEndArrowheadStyle(int value)
```


Définit le type de flèche finale de la ligne.

Voir [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setEndArrowheadWidth(int value) {#setEndArrowheadWidth-int-}
```
public void setEndArrowheadWidth(int value)
```


Définit le type de largeur de la flèche finale de la ligne.

Voir [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setFillType(int value) {#setFillType-int-}
```
public void setFillType(int value)
```


Définit le type de remplissage

Voir [FillType](../../com.aspose.cells/filltype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


Définit les données d'image de la picture.

**Remarks**

Si le format de remplissage n'est pas un format de texture personnalisé, renvoie null.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte[] |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


Spécifie le type de jointure de la ligne.

Voir [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


Représente le motif d'affichage d'une zone.

Voir [FillPattern](../../com.aspose.cells/fillpattern).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPictureFormatType(int value) {#setPictureFormatType-int-}
```
public void setPictureFormatType(int value)
```


Définit le type de format d'image.

Voir [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Définit le remplissage spécifié à un dégradé de couleur prédéfinie. S'applique uniquement à Excel 2007.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Type de couleur prédéfini |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Style d'ombrage du dégradé. |
| variante | int | La variante de dégradé. Peut être une valeur de 1 à 4, correspondant à l'une des quatre variantes dans l'onglet Gradient de la boîte de dialogue Remplissage d'effets. Si le style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2. |

### setScale(double value) {#setScale-double-}
```
public void setScale(double value)
```


Définit l'échelle du format d'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setSetType(int value) {#setSetType-int-}
```
public void setSetType(int value)
```


Obtient le type du jeu de format de remplissage.

Voir [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété FillFormat.FillType. Cette propriété sera supprimée 12 mois plus tard, depuis juillet 2016. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTexture(int value) {#setTexture-int-}
```
public void setTexture(int value)
```


Représente le type de texture pour le remplissage spécifié.

Voir [TextureType](../../com.aspose.cells/texturetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Renvoie ou définit le degré de transparence de la zone sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

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

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Définit le type de remplissage.

Voir [FillType](../../com.aspose.cells/filltype).

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété FillFormat.FillType. Cette propriété sera supprimée 12 mois plus tard, depuis juillet 2016. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setWeight(double value) {#setWeight-double-}
```
public void setWeight(double value)
```


Définit le poids de la ligne en unité de points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

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

