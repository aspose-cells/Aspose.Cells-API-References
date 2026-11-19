---
title: "GridPicture"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente une image unique dans une feuille de calcul."
type: docs
url: /fr/java/com.aspose.gridweb/gridpicture/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridPicture implements IGridSave
```

Encapsule l'objet qui représente une image unique dans une feuille de calcul.
## Méthodes

| Méthode | Description |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Ajoute un hyperlien à la forme. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Déplace l'image vers le coin supérieur droit. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Renvoie ou définit la chaîne de texte descriptive (alternative) de l'objet [GridShape](../../com.aspose.gridweb/gridshape). |
| [getBorderLineColor()](#getBorderLineColor--) | Représente le [Color](../../com.aspose.cells/color) de la bordure d'une image. |
| [getBorderWeight()](#getBorderWeight--) | Obtient l'épaisseur de la bordure d'une image en points (pt). |
| [getBottom()](#getBottom--) | Représente la largeur du décalage vertical de la forme depuis la rangée de son coin inférieur, en unités de pixels. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Obtient les données de l'image. |
| [getHeight()](#getHeight--) | Représente la hauteur de la forme, en unité de pixel. |
| [getHeightCM()](#getHeightCM--) | Représente la hauteur de la forme, en unité de pouces. |
| [getHeightInch()](#getHeightInch--) | Représente la hauteur de la forme, en unité de pouces. |
| [getHeightPt()](#getHeightPt--) | Représente la hauteur de la forme, en unité de points. |
| [getHeightScale()](#getHeightScale--) | Obtient l'échelle de hauteur, en pourcentage de la hauteur originale de l'image. |
| [getHtmlText()](#getHtmlText--) | Obtient la chaîne HTML qui contient des données et certains formats dans cette zone de texte. |
| [getHyperlink()](#getHyperlink--) | Obtient le lien hypertexte de la forme. |
| [getID()](#getID--) | Obtient / Définit l'ID de l'image. |
| [getImageFormat()](#getImageFormat--) | Obtient le format d'image de l'image. |
| [getLeft()](#getLeft--) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pixels. |
| [getLeftCM()](#getLeftCM--) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de centimètres. |
| [getLeftInch()](#getLeftInch--) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pouces. |
| [getLeftToCorner()](#getLeftToCorner--) | Représente le décalage horizontal de la forme depuis le bord gauche de la feuille de calcul, en pixels. |
| [getLinkedCell()](#getLinkedCell--) | Obtient la plage de la feuille de calcul liée à la valeur du contrôle. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Obtient le décalage horizontal de la forme par rapport à la colonne de son coin inférieur droit. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Obtient le décalage vertical de la forme par rapport à la ligne de son coin inférieur droit. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Représente l'index de la colonne du coin inférieur droit. |
| [getLowerRightRow()](#getLowerRightRow--) | Représente l'index de la ligne du coin inférieur droit. |
| [getName()](#getName--) | Obtient le nom de la forme. |
| [getOriginalHeight()](#getOriginalHeight--) | Obtient la hauteur originale de l'image. |
| [getOriginalHeightCM()](#getOriginalHeightCM--) | Obtient la hauteur originale de l'image, en centimètres. |
| [getOriginalHeightInch()](#getOriginalHeightInch--) | Obtient la hauteur originale de l'image, en unités de pouces. |
| [getOriginalWidth()](#getOriginalWidth--) | Obtient la largeur originale de l'image. |
| [getOriginalWidthCM()](#getOriginalWidthCM--) | Obtient la largeur originale de l'image, en unités de centimètres. |
| [getOriginalWidthInch()](#getOriginalWidthInch--) | Obtient la largeur originale de l'image, en unités de pouces. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Indique si la forme est relative à la taille de l'image originale. |
| [getRight()](#getRight--) | Représente la largeur du décalage horizontal de la forme par rapport à la colonne de son coin inférieur droit, en unité de pixels. |
| [getRotationAngle()](#getRotationAngle--) | Obtient la rotation de la forme. |
| [getSourceFullName()](#getSourceFullName--) | Obtient le chemin et le nom du fichier source pour l'image liée. |
| [getText()](#getText--) | Représente la chaîne dans cet objet TextBox. |
| [getTitle()](#getTitle--) | Spécifie le titre (légende) de l’objet forme actuel. |
| [getTop()](#getTop--) | Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pixels. |
| [getTopCM()](#getTopCM--) | Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de centimètres. |
| [getTopInch()](#getTopInch--) | Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pouces. |
| [getTopToCorner()](#getTopToCorner--) | Représente le décalage vertical de la forme depuis le bord supérieur de la feuille de calcul, en pixels. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Obtient le décalage horizontal de la forme depuis la colonne de son coin supérieur gauche. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Obtient le décalage vertical de la forme depuis la ligne de son coin supérieur gauche. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Représente l’indice de colonne du coin supérieur gauche. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Représente l'index de ligne du coin supérieur gauche. |
| [getWidth()](#getWidth--) | Représente la largeur de la forme, en unités de pixels. |
| [getWidthCM()](#getWidthCM--) | Représente la largeur de la forme, en unités de centimètres. |
| [getWidthInch()](#getWidthInch--) | Représente la largeur de la forme, en unités de pouce. |
| [getWidthPt()](#getWidthPt--) | Représente la largeur de la forme, en unités de point. |
| [getWidthScale()](#getWidthScale--) | Obtient l'échelle de largeur, en unité de pourcentage de la largeur d'image originale. |
| [getX()](#getX--) | Obtient le décalage horizontal de la forme depuis le bord gauche de la feuille de calcul, en pixels. |
| [getY()](#getY--) | Obtient le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul, en unités de pixels. |
| [getZOrderPosition()](#getZOrderPosition--) | Renvoie la position d'une forme dans l'ordre Z. |
| [hasLine()](#hasLine--) | Obtient la visibilité de la bordure de ligne de la forme. |
| [hashCode()](#hashCode--) |  |
| [isFlippedVertically()](#isFlippedVertically--) | Obtient si la forme est retournée verticalement. |
| [isGroup()](#isGroup--) | Indique si la forme est un groupe. |
| [isHidden()](#isHidden--) | Indique si l'objet est visible. |
| [isLockAspectRatio()](#isLockAspectRatio--) | Vrai signifie qu'il ne faut pas autoriser les changements de proportion. |
| [isLocked()](#isLocked--) | Vrai si l'objet est verrouillé, Faux si l'objet peut être modifié lorsque la feuille est protégée. |
| [isTextWrapped()](#isTextWrapped--) | Obtient le type d'habillage du texte de la forme qui contient du texte. |
| [move(int upperLeftRow, int upperLeftColumn)](#move-int-int-) | Déplace l'image vers un emplacement spécifié. |
| [moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)](#moveToRange-int-int-int-int-) | Déplace la forme vers une plage spécifiée. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeHyperlink()](#removeHyperlink--) | Supprimer le lien hypertexte de la forme. |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Crée l'image et l'enregistre dans un flux. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Renvoie ou définit la chaîne de texte descriptive (alternative) de l'objet [GridShape](../../com.aspose.gridweb/gridshape). |
| [setBorderLineColor(Color value)](#setBorderLineColor-com.aspose.gridweb.Color-) | Représente le [Color](../../com.aspose.cells/color) de la bordure d'une image. |
| [setBorderWeight(double value)](#setBorderWeight-double-) | Définit l'épaisseur de la bordure d'une image en unités de pt. |
| [setBottom(int value)](#setBottom-int-) | Représente la largeur du décalage vertical de la forme depuis la rangée de son coin inférieur, en unités de pixels. |
| [setData(byte[] value)](#setData-byte---) | Obtient les données de l'image. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Définit si la forme est retournée verticalement. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Définit que la bordure de ligne de la forme est visible. |
| [setHeight(int value)](#setHeight-int-) | Représente la hauteur de la forme, en unité de pixel. |
| [setHeightCM(double value)](#setHeightCM-double-) | Représente la hauteur de la forme, en unité de pouces. |
| [setHeightInch(double value)](#setHeightInch-double-) | Représente la hauteur de la forme, en unité de pouces. |
| [setHeightPt(double value)](#setHeightPt-double-) | Représente la hauteur de la forme, en unité de points. |
| [setHeightScale(int value)](#setHeightScale-int-) | Définit l'échelle de hauteur, en pourcentage de la hauteur de l'image originale. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indique si l'objet est visible. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Définit la chaîne HTML qui contient des données et certains formats dans cette zone de texte. |
| [setID(String value)](#setID-java.lang.String-) | Obtient / Définit l'ID de l'image. |
| [setLeft(int value)](#setLeft-int-) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pixels. |
| [setLeftCM(double value)](#setLeftCM-double-) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de centimètres. |
| [setLeftInch(double value)](#setLeftInch-double-) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pouces. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Représente le décalage horizontal de la forme depuis le bord gauche de la feuille de calcul, en pixels. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Définit la plage de feuille de calcul liée à la valeur du contrôle. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | Vrai signifie qu'il ne faut pas autoriser les changements de proportion. |
| [setLocked(boolean value)](#setLocked-boolean-) | Vrai si l'objet est verrouillé, Faux si l'objet peut être modifié lorsque la feuille est protégée. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Définit le décalage horizontal de la forme depuis la colonne de son coin inférieur droit. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Définit le décalage vertical de la forme depuis la ligne de son coin inférieur droit. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Représente l'index de la colonne du coin inférieur droit. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Représente l'index de la ligne du coin inférieur droit. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom de la forme. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Indique si la forme est relative à la taille de l'image originale. |
| [setRight(int value)](#setRight-int-) | Représente la largeur du décalage horizontal de la forme par rapport à la colonne de son coin inférieur droit, en unité de pixels. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Définit la rotation de la forme. |
| [setSourceFullName(String value)](#setSourceFullName-java.lang.String-) | Définit le chemin et le nom du fichier source pour l'image liée. |
| [setText(String value)](#setText-java.lang.String-) | Représente la chaîne dans cet objet TextBox. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Définit le type d'habillage du texte de la forme contenant du texte. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Spécifie le titre (légende) de l’objet forme actuel. |
| [setTop(int value)](#setTop-int-) | Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pixels. |
| [setTopCM(double value)](#setTopCM-double-) | Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de centimètres. |
| [setTopInch(double value)](#setTopInch-double-) | Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pouces. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Représente le décalage vertical de la forme depuis le bord supérieur de la feuille de calcul, en pixels. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Définit le décalage horizontal de la forme par rapport à la colonne de son coin supérieur gauche. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Définit le décalage vertical de la forme par rapport à la ligne de son coin supérieur gauche. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Représente l’indice de colonne du coin supérieur gauche. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Représente l'index de ligne du coin supérieur gauche. |
| [setWidth(int value)](#setWidth-int-) | Représente la largeur de la forme, en unités de pixels. |
| [setWidthCM(double value)](#setWidthCM-double-) | Représente la largeur de la forme, en unités de centimètres. |
| [setWidthInch(double value)](#setWidthInch-double-) | Représente la largeur de la forme, en unités de pouce. |
| [setWidthPt(double value)](#setWidthPt-double-) | Représente la largeur de la forme, en unités de point. |
| [setWidthScale(int value)](#setWidthScale-int-) | Définit l'échelle de largeur, en pourcentage de la largeur d'origine de l'image. |
| [setX(int value)](#setX-int-) | Définit le décalage horizontal de la forme par rapport à la bordure gauche de la feuille, en pixels. |
| [setY(int value)](#setY-int-) | Définit le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul, en unité de pixels. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Renvoie la position d'une forme dans l'ordre Z. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public GridHyperlink addHyperlink(String address)
```


Ajoute un hyperlien à la forme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| adresse | java.lang.String | Adresse du lien hypertexte. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - Return the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Déplace l'image vers le coin supérieur droit.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | l'index de la ligne. |
| rightColumn | int | l'index de colonne. |

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Renvoie ou définit la chaîne de texte descriptive (alternative) de l'objet [GridShape](../../com.aspose.gridweb/gridshape).

**Returns:**
java.lang.String
### getBorderLineColor() {#getBorderLineColor--}
```
public Color getBorderLineColor()
```


Représente le [Color](../../com.aspose.cells/color) de la bordure d'une image.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderWeight() {#getBorderWeight--}
```
public double getBorderWeight()
```


Obtient l'épaisseur de la bordure d'une image en points (pt).

**Returns:**
double
### getBottom() {#getBottom--}
```
public int getBottom()
```


Représente la largeur du décalage vertical de la forme depuis la rangée de son coin inférieur, en unités de pixels.

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


Obtient les données de l'image.

**Returns:**
byte[]
### getHeight() {#getHeight--}
```
public int getHeight()
```


Représente la hauteur de la forme, en unité de pixel.

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


Représente la hauteur de la forme, en unité de pouces.

**Returns:**
double
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


Représente la hauteur de la forme, en unité de pouces.

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


Représente la hauteur de la forme, en unité de points.

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


Obtient l'échelle de hauteur, en pourcentage de la hauteur originale de l'image. Si la forme n'est pas une image, la propriété HeightScale ne renvoie que 100 ;

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


Obtient la chaîne HTML qui contient des données et certains formats dans cette zone de texte.

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public GridHyperlink getHyperlink()
```


Obtient le lien hypertexte de la forme.

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink)
### getID() {#getID--}
```
public String getID()
```


Obtient / Définit l'ID de l'image.

**Returns:**
java.lang.String
### getImageFormat() {#getImageFormat--}
```
public int getImageFormat()
```


Obtient le format d'image de l'image.

Voir [GridImageType](../../com.aspose.gridweb/gridimagetype).

**Returns:**
int
### getLeft() {#getLeft--}
```
public int getLeft()
```


Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pixels.

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de centimètres.

**Returns:**
double
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pouces.

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Représente le décalage horizontal de la forme depuis le bord gauche de la feuille de calcul, en pixels.

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Obtient la plage de la feuille de calcul liée à la valeur du contrôle.

**Returns:**
java.lang.String
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


Obtient le décalage horizontal de la forme à partir de la colonne de son coin inférieur droit. La plage de valeurs est de 0 à 1024.

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


Obtient le décalage vertical de la forme à partir de la ligne de son coin inférieur droit. La plage de valeurs est de 0 à 256.

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


Représente l'index de la colonne du coin inférieur droit.

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


Représente l'index de la ligne du coin inférieur droit.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtient le nom de la forme.

**Returns:**
java.lang.String
### getOriginalHeight() {#getOriginalHeight--}
```
public int getOriginalHeight()
```


Obtient la hauteur originale de l'image.

**Returns:**
int
### getOriginalHeightCM() {#getOriginalHeightCM--}
```
public double getOriginalHeightCM()
```


Obtient la hauteur originale de l'image, en centimètres.

**Returns:**
double
### getOriginalHeightInch() {#getOriginalHeightInch--}
```
public double getOriginalHeightInch()
```


Obtient la hauteur originale de l'image, en unités de pouces.

**Returns:**
double
### getOriginalWidth() {#getOriginalWidth--}
```
public int getOriginalWidth()
```


Obtient la largeur originale de l'image.

**Returns:**
int
### getOriginalWidthCM() {#getOriginalWidthCM--}
```
public double getOriginalWidthCM()
```


Obtient la largeur originale de l'image, en unités de centimètres.

**Returns:**
double
### getOriginalWidthInch() {#getOriginalWidthInch--}
```
public double getOriginalWidthInch()
```


Obtient la largeur originale de l'image, en unités de pouces.

**Returns:**
double
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


Indique si la forme est relative à la taille de l'image originale.

**Returns:**
boolean
### getRight() {#getRight--}
```
public int getRight()
```


Représente la largeur du décalage horizontal de la forme par rapport à la colonne de son coin inférieur droit, en unité de pixels.

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


Obtient la rotation de la forme.

**Returns:**
double
### getSourceFullName() {#getSourceFullName--}
```
public String getSourceFullName()
```


Obtient le chemin et le nom du fichier source pour l'image liée.

**Remarks**

La valeur par défaut est une chaîne vide. Si SourceFullName n'est pas une chaîne vide, l'image est liée. Si SourceFullName n'est pas une chaîne vide, mais que Data est null, alors l'image est liée et n'est pas stockée dans le fichier.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Représente la chaîne dans cet objet TextBox.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Spécifie le titre (légende) de l’objet forme actuel.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pixels.

**Remarks**

Si la forme se trouve dans le graphique, représente le décalage vertical de la forme par rapport à sa bordure supérieure.

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de centimètres.

**Returns:**
double
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pouces.

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Représente le décalage vertical de la forme depuis le bord supérieur de la feuille de calcul, en pixels.

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


Obtient le décalage horizontal de la forme à partir de la colonne de son coin supérieur gauche. La plage de valeurs est de 0 à 1024.

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


Obtient le décalage vertical de la forme à partir de la ligne de son coin supérieur gauche. La plage de valeurs est de 0 à 256.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Représente l’indice de colonne du coin supérieur gauche.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Représente l'index de ligne du coin supérieur gauche.

**Remarks**

Si la forme est dans une forme ou dans un groupe, UpperLeftRow sera ignoré.

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Représente la largeur de la forme, en unités de pixels.

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


Représente la largeur de la forme, en unités de centimètres.

**Returns:**
double
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


Représente la largeur de la forme, en unités de pouce.

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


Représente la largeur de la forme, en unités de point.

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


Obtient l'échelle de largeur, en pourcentage de la largeur originale de l'image. Si la forme n'est pas une image, la propriété WidthScale ne renvoie que 100 ;

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


Obtient le décalage horizontal de la forme depuis le bord gauche de la feuille de calcul, en pixels.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Obtient le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul, en unités de pixels.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Renvoie la position d'une forme dans l'ordre Z.

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


Obtient la visibilité de la bordure de ligne de la forme.

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


Obtient si la forme est retournée verticalement.

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


Indique si la forme est un groupe.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indique si l'objet est visible.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


Vrai signifie qu'il ne faut pas autoriser les changements de proportion.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Vrai si l'objet est verrouillé, Faux si l'objet peut être modifié lorsque la feuille est protégée.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Obtient le type d'habillage du texte de la forme qui contient du texte.

**Returns:**
boolean
### move(int upperLeftRow, int upperLeftColumn) {#move-int-int-}
```
public void move(int upperLeftRow, int upperLeftColumn)
```


Déplace l'image vers un emplacement spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Indice de ligne en haut à gauche. |
| upperLeftColumn | int | Indice de colonne en haut à gauche. |

### moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)
```


Déplace la forme vers une plage spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Indice de ligne en haut à gauche. |
| upperLeftColumn | int | Indice de colonne en haut à gauche. |
| lowerRightRow | int | Indice de ligne en bas à droite |
| lowerRightColumn | int | Indice de colonne en bas à droite |

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


Supprimer le lien hypertexte de la forme.

### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


Crée l'image et l'enregistre dans un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Renvoie ou définit la chaîne de texte descriptive (alternative) de l'objet [GridShape](../../com.aspose.gridweb/gridshape).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setBorderLineColor(Color value) {#setBorderLineColor-com.aspose.gridweb.Color-}
```
public void setBorderLineColor(Color value)
```


Représente le [Color](../../com.aspose.cells/color) de la bordure d'une image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderWeight(double value) {#setBorderWeight-double-}
```
public void setBorderWeight(double value)
```


Définit l'épaisseur de la bordure d'une image en unités de pt.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


Représente la largeur du décalage vertical de la forme depuis la rangée de son coin inférieur, en unités de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setData(byte[] value) {#setData-byte---}
```
public void setData(byte[] value)
```


Obtient les données de l'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte[] |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


Définit si la forme est retournée verticalement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasLine(boolean value) {#setHasLine-boolean-}
```
public void setHasLine(boolean value)
```


Définit que la bordure de ligne de la forme est visible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Représente la hauteur de la forme, en unité de pixel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


Représente la hauteur de la forme, en unité de pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


Représente la hauteur de la forme, en unité de pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setHeightPt(double value) {#setHeightPt-double-}
```
public void setHeightPt(double value)
```


Représente la hauteur de la forme, en unité de points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setHeightScale(int value) {#setHeightScale-int-}
```
public void setHeightScale(int value)
```


Définit l'échelle de hauteur, en pourcentage de la hauteur d'image d'origine. Si la forme n'est pas une image, la propriété HeightScale renvoie uniquement 100 ;

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indique si l'objet est visible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHtmlText(String value) {#setHtmlText-java.lang.String-}
```
public void setHtmlText(String value)
```


Définit la chaîne HTML qui contient des données et certains formats dans cette zone de texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


Obtient / Définit l'ID de l'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setLeft(int value) {#setLeft-int-}
```
public void setLeft(int value)
```


Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLeftCM(double value) {#setLeftCM-double-}
```
public void setLeftCM(double value)
```


Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de centimètres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setLeftInch(double value) {#setLeftInch-double-}
```
public void setLeftInch(double value)
```


Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


Représente le décalage horizontal de la forme depuis le bord gauche de la feuille de calcul, en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Définit la plage de feuille de calcul liée à la valeur du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


Vrai signifie qu'il ne faut pas autoriser les changements de proportion.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Vrai si l'objet est verrouillé, Faux si l'objet peut être modifié lorsque la feuille est protégée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


Définit le décalage horizontal de la forme à partir de la colonne de son coin inférieur droit. La plage de valeurs est de 0 à 1024.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


Définit le décalage vertical de la forme à partir de la ligne de son coin inférieur droit. La plage de valeurs est de 0 à 256.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLowerRightColumn(int value) {#setLowerRightColumn-int-}
```
public void setLowerRightColumn(int value)
```


Représente l'index de la colonne du coin inférieur droit.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLowerRightRow(int value) {#setLowerRightRow-int-}
```
public void setLowerRightRow(int value)
```


Représente l'index de la ligne du coin inférieur droit.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Définit le nom de la forme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setRelativeToOriginalPictureSize(boolean value) {#setRelativeToOriginalPictureSize-boolean-}
```
public void setRelativeToOriginalPictureSize(boolean value)
```


Indique si la forme est relative à la taille de l'image originale.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRight(int value) {#setRight-int-}
```
public void setRight(int value)
```


Représente la largeur du décalage horizontal de la forme par rapport à la colonne de son coin inférieur droit, en unité de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Définit la rotation de la forme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setSourceFullName(String value) {#setSourceFullName-java.lang.String-}
```
public void setSourceFullName(String value)
```


Définit le chemin et le nom du fichier source pour l'image liée.

**Remarks**

La valeur par défaut est une chaîne vide. Si SourceFullName n'est pas une chaîne vide, l'image est liée. Si SourceFullName n'est pas une chaîne vide, mais que Data est null, alors l'image est liée et n'est pas stockée dans le fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Représente la chaîne dans cet objet TextBox.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Définit le type d'habillage du texte de la forme contenant du texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Spécifie le titre (légende) de l’objet forme actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTop(int value) {#setTop-int-}
```
public void setTop(int value)
```


Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pixels.

**Remarks**

Si la forme se trouve dans le graphique, représente le décalage vertical de la forme par rapport à sa bordure supérieure.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTopCM(double value) {#setTopCM-double-}
```
public void setTopCM(double value)
```


Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de centimètres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setTopInch(double value) {#setTopInch-double-}
```
public void setTopInch(double value)
```


Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


Représente le décalage vertical de la forme depuis le bord supérieur de la feuille de calcul, en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


Définit le décalage horizontal de la forme à partir de la colonne de son coin supérieur gauche. La plage de valeurs est de 0 à 1024.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


Définit le décalage vertical de la forme à partir de la ligne de son coin supérieur gauche. La plage de valeurs est de 0 à 256.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setUpperLeftColumn(int value) {#setUpperLeftColumn-int-}
```
public void setUpperLeftColumn(int value)
```


Représente l’indice de colonne du coin supérieur gauche.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setUpperLeftRow(int value) {#setUpperLeftRow-int-}
```
public void setUpperLeftRow(int value)
```


Représente l'index de ligne du coin supérieur gauche.

**Remarks**

Si la forme est dans une forme ou dans un groupe, UpperLeftRow sera ignoré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Représente la largeur de la forme, en unités de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


Représente la largeur de la forme, en unités de centimètres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


Représente la largeur de la forme, en unités de pouce.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWidthPt(double value) {#setWidthPt-double-}
```
public void setWidthPt(double value)
```


Représente la largeur de la forme, en unités de point.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWidthScale(int value) {#setWidthScale-int-}
```
public void setWidthScale(int value)
```


Définit l'échelle de largeur, en pourcentage de la largeur d'image d'origine. Si la forme n'est pas une image, la propriété WidthScale renvoie uniquement 100 ;

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Définit le décalage horizontal de la forme par rapport à la bordure gauche de la feuille, en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Définit le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul, en unité de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


Renvoie la position d'une forme dans l'ordre Z.

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

