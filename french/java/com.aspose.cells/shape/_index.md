---
title: "Forme"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente l'objet msodrawing."
type: docs
url: /fr/java/com.aspose.cells/shape/
---

**Inheritance:**
java.lang.Object
```
public class Shape
```

Représente l'objet msodrawing.

**Example**

```
         //Initialize a new workbook.
         Workbook book = new Workbook();
 
         //Add a shape.(e.g rectangle)
         Shape shape = book.getWorksheets().get(0).getShapes().addRectangle(2, 0, 2, 0, 130, 130);
 
         //do your business
 
         //Save the excel file.
         book.save("exmaple.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Ajoute un hyperlien à la forme. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Déplace l'image vers le coin supérieur droit. |
| [calculateTextSize()](#calculateTextSize--) | Recalculer la zone de texte |
| [characters(int startIndex, int length)](#characters-int-int-) | Renvoie un objet Characters qui représente une plage de caractères dans le texte. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fitToTextSize()](#fitToTextSize--) | Recalculer une zone de texte adaptée à l'affichage de tout le contenu texte. |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Formate certains caractères avec le paramètre de police. |
| [getActiveXControl()](#getActiveXControl--) | Obtient le contrôle ActiveX. |
| [getActualBox()](#getActualBox--) | Obtenir la position et la taille réelles de la forme (après application de la rotation, du retournement, etc.) |
| [getActualLowerRightRow()](#getActualLowerRightRow--) | Obtenir la ligne inférieure réelle. |
| [getAlternativeText()](#getAlternativeText--) | Renvoie ou définit la chaîne de texte descriptive (alternative) de l'objet [Shape](../../com.aspose.cells/shape). |
| [getAnchorType()](#getAnchorType--) | Obtient le type de l'espace réservé d'ancrage de forme. |
| [getAutoShapeType()](#getAutoShapeType--) | Obtient le type de forme automatique. |
| [getBottom()](#getBottom--) | Représente la largeur du décalage vertical de la forme depuis la rangée de son coin inférieur, en unités de pixels. |
| [getCharacters()](#getCharacters--) | Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte. |
| [getClass()](#getClass--) |  |
| [getConnectionPoints()](#getConnectionPoints--) | Obtenez les points de connexion |
| [getControlData()](#getControlData--) | Obtient les données du contrôle. |
| [getCreateId()](#getCreateId--) | Obtient l'ID de création pour cette forme. |
| [getFill()](#getFill--) | Renvoie un objet [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--) qui contient les propriétés de format de remplissage pour la forme spécifiée. |
| [getFillFormat()](#getFillFormat--) | Renvoie un objet MsoFillFormat qui contient les propriétés de format de remplissage pour la forme spécifiée. |
| [getFont()](#getFont--) | Représente la police de la forme. |
| [getFormatPicture()](#getFormatPicture--) | Obtient les options du format d'image. |
| [getGeometry()](#getGeometry--) | Obtient la géométrie |
| [getGlow()](#getGlow--) | Représente un objet [GlowEffect](../../com.aspose.cells/gloweffect) qui spécifie l'effet de lueur pour l'élément de graphique ou la forme. |
| [getGroup()](#getGroup--) | Obtient le groupe de formes qui contient cette forme. |
| [getHeight()](#getHeight--) | Représente la hauteur de la forme, en unité de pixel. |
| [getHeightCM()](#getHeightCM--) | Représente la hauteur de la forme, en unité de centimètres. |
| [getHeightInShape()](#getHeightInShape--) | Représente le décalage vertical de la forme depuis la bordure supérieure de la forme parente, en unité de 1/4000 de la hauteur de la forme parente. |
| [getHeightInch()](#getHeightInch--) | Représente la hauteur de la forme, en unité de pouces. |
| [getHeightPt()](#getHeightPt--) | Représente la hauteur de la forme, en unité de points. |
| [getHeightScale()](#getHeightScale--) | Obtient l'échelle de hauteur, en pourcentage de la hauteur originale de l'image. |
| [getHtmlText()](#getHtmlText--) | Obtient la chaîne HTML qui contient les données et certains formats dans cette zone de texte. |
| [getHyperlink()](#getHyperlink--) | Obtient le lien hypertexte de la forme. |
| [getId()](#getId--) | Obtient l'identifiant de cette forme. |
| [getInputRange()](#getInputRange--) | Obtient la plage de feuille de calcul utilisée pour remplir la zone de liste déroulante spécifiée. |
| [getInputRange(boolean isR1C1, boolean isLocal)](#getInputRange-boolean-boolean-) | Obtient la plage utilisée pour remplir le contrôle. |
| [getLeft()](#getLeft--) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pixels. |
| [getLeftCM()](#getLeftCM--) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de centimètres. |
| [getLeftInShape()](#getLeftInShape--) | Représente le décalage horizontal de la forme par rapport à la bordure gauche de la forme parent, en unité de 1/4000 de la largeur de la forme parent. |
| [getLeftInch()](#getLeftInch--) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pouces. |
| [getLeftToCorner()](#getLeftToCorner--) | Obtient le décalage horizontal de la forme par rapport à la bordure gauche de la feuille de calcul. |
| [getLine()](#getLine--) | Obtient le style de ligne |
| [getLineFormat()](#getLineFormat--) | Renvoie un objet MsoLineFormat qui contient les propriétés de formatage de ligne pour la forme spécifiée. |
| [getLinkedCell()](#getLinkedCell--) | Obtient la plage de la feuille de calcul liée à la valeur du contrôle. |
| [getLinkedCell(boolean isR1C1, boolean isLocal)](#getLinkedCell-boolean-boolean-) | Obtient la plage liée à la valeur du contrôle. |
| [getLockedProperty(int type)](#getLockedProperty-int-) | Obtient la valeur de la propriété verrouillée. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Obtient le décalage horizontal de la forme par rapport à la colonne de son coin inférieur droit. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Obtient le décalage vertical de la forme par rapport à la ligne de son coin inférieur droit. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Représente l'index de la colonne du coin inférieur droit. |
| [getLowerRightRow()](#getLowerRightRow--) | Représente l'index de la ligne du coin inférieur droit. |
| [getMacroName()](#getMacroName--) | Obtient le nom de la macro. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Obtient le type de dessin. |
| [getName()](#getName--) | Obtient le nom de la forme. |
| [getPaths()](#getPaths--) | Obtient les chemins d'une forme géométrique personnalisée. |
| [getPlacement()](#getPlacement--) | Représente la façon dont l'objet de dessin est attaché aux cellules en dessous. |
| [getReflection()](#getReflection--) | Représente un objet [ReflectionEffect](../../com.aspose.cells/reflectioneffect) qui spécifie l'effet de réflexion pour l'élément de graphique ou la forme. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Indique si la forme est relative à la taille de l'image originale. |
| [getResultOfSmartArt()](#getResultOfSmartArt--) | Conversion du SmartArt en formes groupées. |
| [getRichFormattings()](#getRichFormattings--) | Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte. |
| [getRight()](#getRight--) | Représente la largeur du décalage horizontal de la forme par rapport à la colonne de son coin inférieur droit, en unité de pixels. |
| [getRotationAngle()](#getRotationAngle--) | Obtient la rotation de la forme. |
| [getShadowEffect()](#getShadowEffect--) | Représente un objet [ShadowEffect](../../com.aspose.cells/shadoweffect) qui spécifie l'effet d'ombre pour l'élément de graphique ou la forme. |
| [getSoftEdges()](#getSoftEdges--) | Obtient le rayon du flou à appliquer aux bords, en unité de points. |
| [getSpid()](#getSpid--) | Spécifie un identifiant de chaîne optionnel qu’une application peut utiliser pour identifier la forme particulière. |
| [getSpt()](#getSpt--) | Spécifie un nombre optionnel qu’une application peut utiliser pour associer la forme particulière à un type de forme défini. |
| [getText()](#getText--) | Obtient le texte de cette forme. |
| [getTextBody()](#getTextBody--) | Obtient le paramètre du texte de la forme. |
| [getTextBoxOptions()](#getTextBoxOptions--) | Obtient les informations de texte dans la forme |
| [getTextDirection()](#getTextDirection--) | Obtient la direction du flux de texte pour cet objet. |
| [getTextEffect()](#getTextEffect--) | Renvoie un objet TextEffectFormat qui contient les propriétés de mise en forme d’effet de texte pour la forme spécifiée. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Obtient le type d’alignement horizontal du texte de la forme. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Obtient le type de dépassement horizontal du texte de la forme qui contient du texte. |
| [getTextOptions()](#getTextOptions--) | Représente les options de texte de la forme. |
| [getTextOrientationType()](#getTextOrientationType--) | Obtient le type d’orientation du texte de la forme. |
| [getTextShapeType()](#getTextShapeType--) | Obtient le type de forme texte prédéfini. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Obtient le type d’alignement vertical du texte de la forme. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Obtient le type de dépassement vertical du texte de la forme qui contient du texte. |
| [getThreeDFormat()](#getThreeDFormat--) | Obtient le format 3D de la forme. |
| [getTitle()](#getTitle--) | Spécifie le titre (légende) de l’objet forme actuel. |
| [getTop()](#getTop--) | Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pixels. |
| [getTopCM()](#getTopCM--) | Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de centimètres. |
| [getTopInShape()](#getTopInShape--) | Représente le décalage vertical de la forme depuis la bordure supérieure de la forme parent, en unité de 1/4000 de la hauteur de la forme parent. |
| [getTopInch()](#getTopInch--) | Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pouces. |
| [getTopToCorner()](#getTopToCorner--) | Obtient le décalage vertical de la forme depuis la bordure supérieure de la feuille de calcul, en unité de pixels. |
| [getType()](#getType--) | Obtient le type de forme automatique. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Obtient le décalage horizontal de la forme depuis la colonne de son coin supérieur gauche. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Obtient le décalage vertical de la forme depuis la ligne de son coin supérieur gauche. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Représente l’indice de colonne du coin supérieur gauche. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Représente l'index de la ligne supérieure. |
| [getWidth()](#getWidth--) | Représente la largeur de la forme, en unités de pixels. |
| [getWidthCM()](#getWidthCM--) | Représente la largeur de la forme, en unités de centimètres. |
| [getWidthInShape()](#getWidthInShape--) | Représente la largeur de la forme, en unités de 1/4000 de la forme parente. |
| [getWidthInch()](#getWidthInch--) | Représente la largeur de la forme, en unités de pouce. |
| [getWidthPt()](#getWidthPt--) | Représente la largeur de la forme, en unités de point. |
| [getWidthScale()](#getWidthScale--) | Obtient l'échelle de largeur, en unité de pourcentage de la largeur d'image originale. |
| [getWorksheet()](#getWorksheet--) | Obtient l'objet [Worksheet](../../com.aspose.cells/worksheet) qui contient cette forme. |
| [getX()](#getX--) | Obtient le décalage horizontal de la forme par rapport à la bordure gauche de la feuille de calcul, en unités de pixels. |
| [getY()](#getY--) | Obtient le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul, en unités de pixels. |
| [getZOrderPosition()](#getZOrderPosition--) | Renvoie la position d'une forme dans l'ordre Z. |
| [hasLine()](#hasLine--) | Obtient la visibilité de la bordure de ligne de la forme. |
| [hashCode()](#hashCode--) |  |
| [isAspectRatioLocked()](#isAspectRatioLocked--) | Vrai signifie que le rapport d'aspect de la forme est verrouillé. |
| [isDecorative()](#isDecorative--) | Indique si l'objet est décoratif. |
| [isEquation()](#isEquation--) | Indique si la forme ne contient qu'une équation. |
| [isFilled()](#isFilled--) | Indique si le format de remplissage est visible. |
| [isFlippedHorizontally()](#isFlippedHorizontally--) | Obtient si la forme est retournée horizontalement. |
| [isFlippedVertically()](#isFlippedVertically--) | Obtient si la forme est retournée verticalement. |
| [isGroup()](#isGroup--) | Indique si cette forme est une forme groupée. |
| [isHidden()](#isHidden--) | Indique si l'objet est visible. |
| [isInGroup()](#isInGroup--) | Indique si la forme est groupée. |
| [isLockAspectRatio()](#isLockAspectRatio--) | Vrai signifie que le rapport d'aspect de la forme est verrouillé. |
| [isLocked()](#isLocked--) | Vrai signifie que l'objet ne peut pas être modifié lorsque la feuille est protégée. |
| [isPrintable()](#isPrintable--) | Indique si l'objet est imprimable. |
| [isRichText()](#isRichText--) | Indique si le texte est du texte enrichi. |
| [isSameSetting(Object obj)](#isSameSetting-java.lang.Object-) | Renvoie si la forme est identique. |
| [isSmartArt()](#isSmartArt--) | Indique si la forme est un SmartArt. |
| [isTextWrapped()](#isTextWrapped--) | Obtient le type d'habillage du texte de la forme qui contient du texte. |
| [isWordArt()](#isWordArt--) | Indique si cette forme est un WordArt. |
| [moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)](#moveToRange-int-int-int-int-) | Déplace la forme vers une plage spécifiée. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeActiveXControl()](#removeActiveXControl--) | Supprime le contrôle ActiveX. |
| [removeHyperlink()](#removeHyperlink--) | Supprime le lien hypertexte de la forme. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Renvoie ou définit la chaîne de texte descriptive (alternative) de l'objet [Shape](../../com.aspose.cells/shape). |
| [setAnchorType(int value)](#setAnchorType-int-) | Définit le type de l'espace réservé d'ancrage de la forme. |
| [setAspectRatioLocked(boolean value)](#setAspectRatioLocked-boolean-) | Vrai signifie que le rapport d'aspect de la forme est verrouillé. |
| [setAutoShapeType(int value)](#setAutoShapeType-int-) | Définit le type de forme automatique. |
| [setBottom(int value)](#setBottom-int-) | Représente la largeur du décalage vertical de la forme depuis la rangée de son coin inférieur, en unités de pixels. |
| [setCreateId(UUID value)](#setCreateId-java.util.UUID-) | Définit l'ID de création pour cette forme. |
| [setDecorative(boolean value)](#setDecorative-boolean-) | Indique si l'objet est décoratif. |
| [setFilled(boolean value)](#setFilled-boolean-) | Indique si le format de remplissage est visible. |
| [setFlippedHorizontally(boolean value)](#setFlippedHorizontally-boolean-) | Définit si la forme est retournée horizontalement. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Définit si la forme est retournée verticalement. |
| [setFont(Font value)](#setFont-com.aspose.cells.Font-) | Représente la police de la forme. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Définit que la bordure de ligne de la forme est visible. |
| [setHeight(int value)](#setHeight-int-) | Représente la hauteur de la forme, en unité de pixel. |
| [setHeightCM(double value)](#setHeightCM-double-) | Représente la hauteur de la forme, en unité de centimètres. |
| [setHeightInShape(int value)](#setHeightInShape-int-) | Représente le décalage vertical de la forme depuis la bordure supérieure de la forme parente, en unité de 1/4000 de la hauteur de la forme parente. |
| [setHeightInch(double value)](#setHeightInch-double-) | Représente la hauteur de la forme, en unité de pouces. |
| [setHeightPt(double value)](#setHeightPt-double-) | Représente la hauteur de la forme, en unité de points. |
| [setHeightScale(int value)](#setHeightScale-int-) | Définit l'échelle de hauteur, en pourcentage de la hauteur de l'image originale. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indique si l'objet est visible. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Définit la chaîne HTML qui contient des données et certains formats dans cette zone de texte. |
| [setInputRange(String value)](#setInputRange-java.lang.String-) | Définit la plage de feuille de calcul utilisée pour remplir la zone combinée spécifiée. |
| [setInputRange(String formula, boolean isR1C1, boolean isLocal)](#setInputRange-java.lang.String-boolean-boolean-) | Définit la plage utilisée pour remplir le contrôle. |
| [setLeft(int value)](#setLeft-int-) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pixels. |
| [setLeftCM(double value)](#setLeftCM-double-) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de centimètres. |
| [setLeftInShape(int value)](#setLeftInShape-int-) | Représente le décalage horizontal de la forme par rapport à la bordure gauche de la forme parent, en unité de 1/4000 de la largeur de la forme parent. |
| [setLeftInch(double value)](#setLeftInch-double-) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pouces. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Définit le décalage horizontal de la forme par rapport à la bordure gauche de la feuille de calcul. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Définit la plage de feuille de calcul liée à la valeur du contrôle. |
| [setLinkedCell(String formula, boolean isR1C1, boolean isLocal)](#setLinkedCell-java.lang.String-boolean-boolean-) | Définit la plage liée à la valeur du contrôle. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | Vrai signifie que le rapport d'aspect de la forme est verrouillé. |
| [setLocked(boolean value)](#setLocked-boolean-) | Vrai signifie que l'objet ne peut pas être modifié lorsque la feuille est protégée. |
| [setLockedProperty(int type, boolean value)](#setLockedProperty-int-boolean-) | Définit la propriété verrouillée. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Définit le décalage horizontal de la forme depuis la colonne de son coin inférieur droit. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Définit le décalage vertical de la forme depuis la ligne de son coin inférieur droit. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Représente l'index de la colonne du coin inférieur droit. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Représente l'index de la ligne du coin inférieur droit. |
| [setMacroName(String value)](#setMacroName-java.lang.String-) | Définit le nom de la macro. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom de la forme. |
| [setPlacement(int value)](#setPlacement-int-) | Représente la façon dont l'objet de dessin est attaché aux cellules en dessous. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | Indique si l'objet est imprimable. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Indique si la forme est relative à la taille de l'image originale. |
| [setRight(int value)](#setRight-int-) | Représente la largeur du décalage horizontal de la forme par rapport à la colonne de son coin inférieur droit, en unité de pixels. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Définit la rotation de la forme. |
| [setSoftEdges(double value)](#setSoftEdges-double-) | Définit le rayon du flou à appliquer aux bords, en unité de points. |
| [setText(String value)](#setText-java.lang.String-) | Définit le texte de cette forme. |
| [setTextDirection(int value)](#setTextDirection-int-) | Définit la direction du flux de texte pour cet objet. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Définit le type d'alignement horizontal du texte de la forme. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Définit le type de débordement horizontal du texte de la forme contenant du texte. |
| [setTextOptions(TextOptions value)](#setTextOptions-com.aspose.cells.TextOptions-) | Représente les options de texte de la forme. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | Définit le type d'orientation du texte de la forme. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Définit le type de forme texte prédéfini. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Définit le type d'alignement vertical du texte de la forme. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Définit le type de débordement vertical du texte de la forme contenant du texte. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Définit le type d'habillage du texte de la forme contenant du texte. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Spécifie le titre (légende) de l’objet forme actuel. |
| [setTop(int value)](#setTop-int-) | Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pixels. |
| [setTopCM(double value)](#setTopCM-double-) | Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de centimètres. |
| [setTopInShape(int value)](#setTopInShape-int-) | Représente le décalage vertical de la forme depuis la bordure supérieure de la forme parent, en unité de 1/4000 de la hauteur de la forme parent. |
| [setTopInch(double value)](#setTopInch-double-) | Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pouces. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Définit le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul, en unité de pixels. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Définit le décalage horizontal de la forme par rapport à la colonne de son coin supérieur gauche. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Définit le décalage vertical de la forme par rapport à la ligne de son coin supérieur gauche. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Représente l’indice de colonne du coin supérieur gauche. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Représente l'index de la ligne supérieure. |
| [setWidth(int value)](#setWidth-int-) | Représente la largeur de la forme, en unités de pixels. |
| [setWidthCM(double value)](#setWidthCM-double-) | Représente la largeur de la forme, en unités de centimètres. |
| [setWidthInShape(int value)](#setWidthInShape-int-) | Représente la largeur de la forme, en unités de 1/4000 de la forme parente. |
| [setWidthInch(double value)](#setWidthInch-double-) | Représente la largeur de la forme, en unités de pouce. |
| [setWidthPt(double value)](#setWidthPt-double-) | Représente la largeur de la forme, en unités de point. |
| [setWidthScale(int value)](#setWidthScale-int-) | Définit l'échelle de largeur, en pourcentage de la largeur d'origine de l'image. |
| [setX(int value)](#setX-int-) | Définit le décalage horizontal de la forme par rapport à la bordure gauche de la feuille de calcul, en unité de pixels. |
| [setY(int value)](#setY-int-) | Définit le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul, en unité de pixels. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Renvoie la position d'une forme dans l'ordre Z. |
| [toFrontOrBack(int orders)](#toFrontOrBack-int-) | Place la forme au premier plan ou l'envoie à l'arrière-plan. |
| [toImage(OutputStream stream, ImageFormat imageFormat)](#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-) | Crée l'image de la forme et l'enregistre dans un flux au format spécifié. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Enregistre la forme dans un flux. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Enregistre la forme dans un fichier. |
| [toString()](#toString--) |  |
| [updateSelectedValue()](#updateSelectedValue--) | Met à jour la valeur sélectionnée avec la valeur de la cellule liée. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public Hyperlink addHyperlink(String address)
```


Ajoute un hyperlien à la forme.

**Example**

```
         Hyperlink hyperlink = shape.addHyperlink("https://www.aspose.com/");
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| adresse | java.lang.String | Adresse du lien hypertexte. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - Returns the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Déplace l'image vers le coin supérieur droit.

**Example**

```
         shape.alignTopRightCorner(2, 5);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | l'index de la ligne. |
| rightColumn | int | l'index de colonne. |

### calculateTextSize() {#calculateTextSize--}
```
public int[] calculateTextSize()
```


Recalculer la zone de texte

**Example**

```
         //The size of the text area is:w=size[0],h=size[1]
         int[] size = shape.calculateTextSize();
```

**Returns:**
int[] - Taille du texte dans un tableau (largeur et hauteur).
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Renvoie un objet Characters qui représente une plage de caractères dans le texte.

**Remarks**

Cette méthode ne fonctionne que sur une forme avec titre.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | int | L'index du début du caractère. |
| length | int | Le nombre de caractères. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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
### fitToTextSize() {#fitToTextSize--}
```
public void fitToTextSize()
```


Recalculer une zone de texte adaptée à l'affichage de tout le contenu texte.

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


Formate certains caractères avec le paramètre de police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | int | L'index de départ. |
| length | int | La longueur. |
| font | [Font](../../com.aspose.cells/font) | Le paramètre de police. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Le drapeau du paramètre de police. |

### getActiveXControl() {#getActiveXControl--}
```
public ActiveXControl getActiveXControl()
```


Obtient le contrôle ActiveX.

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


Obtenir la position et la taille réelles de la forme (après application de la rotation, du retournement, etc.)

**Remarks**

Remarque : L'interface n'est pas entièrement fonctionnelle, en particulier les informations de localisation ne sont pas correctes. Il est recommandé de ne pas utiliser cette interface tant que la fonction n'est pas terminée.

**Example**

```
         float[] box = shape.getActualBox();
         System.out.println("x = " + box[0]);
         System.out.println("y = " + box[1]);
         System.out.println("w = " + box[2]);
         System.out.println("h = " + box[3]);
```

**Returns:**
float[] - Retourne la position et la taille dans l'ordre x, y, w, h
### getActualLowerRightRow() {#getActualLowerRightRow--}
```
public int getActualLowerRightRow()
```


Obtenir la ligne inférieure réelle.

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


Renvoie ou définit la chaîne de texte descriptive (alternative) de l'objet [Shape](../../com.aspose.cells/shape).

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


Obtient le type de l'espace réservé d'ancrage de forme.

Voir [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

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


Obtient le type de forme automatique.

Voir [AutoShapeType](../../com.aspose.cells/autoshapetype).

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


Représente la largeur du décalage vertical de la forme depuis la rangée de son coin inférieur, en unités de pixels.

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


Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. Veuillez plutôt utiliser la méthode Shape.GetRichFormattings(). Cette méthode sera supprimée 12 mois après, depuis novembre 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Returns:**
java.util.ArrayList - Tous les objets Characters
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


Obtenez les points de connexion

**Example**

```
         float[][] points = shape.getConnectionPoints();
```

**Returns:**
float[][] - paires [X,Y] du point de connexion. Chaque élément est un tableau float[2], [0] représente x et [1] représente y.
### getControlData() {#getControlData--}
```
public byte[] getControlData()
```


Obtient les données du contrôle.

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


Obtient l'ID de création pour cette forme.

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


Renvoie un objet [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--) qui contient les propriétés de format de remplissage pour la forme spécifiée.

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


Renvoie un objet MsoFillFormat qui contient les propriétés de format de remplissage pour la forme spécifiée.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété Shape.Fill. Cette propriété sera supprimée 12 mois après, depuis juillet 2016. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
[MsoFillFormat](../../com.aspose.cells/msofillformat)
### getFont() {#getFont--}
```
public Font getFont()
```


Représente la police de la forme.

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


Obtient les options du format d'image.

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


Obtient la géométrie

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


Représente un objet [GlowEffect](../../com.aspose.cells/gloweffect) qui spécifie l'effet de lueur pour l'élément de graphique ou la forme.

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


Obtient le groupe de formes qui contient cette forme.

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


Représente la hauteur de la forme, en unité de pixel.

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


Représente la hauteur de la forme, en unité de centimètres.

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


Représente le décalage vertical de la forme depuis la bordure supérieure de la forme parente, en unité de 1/4000 de la hauteur de la forme parente.

**Remarks**

S'applique uniquement lorsque cette forme se trouve dans le groupe ou le graphique.

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


Représente la hauteur de la forme, en unité de pouces.

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


Représente la hauteur de la forme, en unité de points.

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


Obtient l'échelle de hauteur, en pourcentage de la hauteur originale de l'image. Si la forme n'est pas une image, la propriété HeightScale ne renvoie que 100 ;

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


Obtient la chaîne HTML qui contient les données et certains formats dans cette zone de texte.

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


Obtient le lien hypertexte de la forme.

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


Obtient l'identifiant de cette forme.

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


Obtient la plage de feuille de calcul utilisée pour remplir la zone de liste déroulante spécifiée.

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


Obtient la plage utilisée pour remplir le contrôle.

**Example**

```
         String range = shape.getInputRange(false, true);
         //If successful, a value like "$A$1:$A$3" will be returned
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |

**Returns:**
java.lang.String - La plage utilisée pour remplir le contrôle.
### getLeft() {#getLeft--}
```
public int getLeft()
```


Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pixels.

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


Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de centimètres.

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


Représente le décalage horizontal de la forme par rapport à la bordure gauche de la forme parent, en unité de 1/4000 de la largeur de la forme parent.

**Remarks**

S'applique uniquement lorsque cette forme se trouve dans le groupe ou le graphique.

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


Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pouces.

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


Obtient le décalage horizontal de la forme par rapport à la bordure gauche de la feuille de calcul.

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


Obtient le style de ligne

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


Renvoie un objet MsoLineFormat qui contient les propriétés de formatage de ligne pour la forme spécifiée.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Line. Cette propriété sera supprimée 12 mois plus tard, depuis juillet 2016. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
[MsoLineFormat](../../com.aspose.cells/msolineformat)
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Obtient la plage de la feuille de calcul liée à la valeur du contrôle.

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


Obtient la plage liée à la valeur du contrôle.

**Example**

```
         //You may get results like '$A$1'
         String link = shape.getLinkedCell(false, false);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |

**Returns:**
java.lang.String - La plage liée à la valeur du contrôle.
### getLockedProperty(int type) {#getLockedProperty-int-}
```
public boolean getLockedProperty(int type)
```


Obtient la valeur de la propriété verrouillée.

**Example**

```
         int noAdjustHandles = 0;
         if (shape.getLockedProperty(ShapeLockType.ADJUST_HANDLES))
             noAdjustHandles = 1;
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). Le type de la propriété locked de la forme. |

**Returns:**
boolean - Renvoie la valeur de la propriété locked.
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


Obtient le décalage horizontal de la forme par rapport à la colonne de son coin inférieur droit.

**Remarks**

La plage de valeurs est de 0 à 1024.

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


Obtient le décalage vertical de la forme par rapport à la ligne de son coin inférieur droit.

**Remarks**

La plage de valeurs est de 0 à 256.

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


Représente l'index de la colonne du coin inférieur droit.

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


Représente l'index de la ligne du coin inférieur droit.

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


Obtient le nom de la macro.

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


Obtient le type de dessin.

Voir [MsoDrawingType](../../com.aspose.cells/msodrawingtype).

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


Obtient le nom de la forme.

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


Obtient les chemins d'une forme géométrique personnalisée.

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


Représente la façon dont l'objet de dessin est attaché aux cellules en dessous. La propriété contrôle le placement d'un objet sur une feuille de calcul.

Voir [PlacementType](../../com.aspose.cells/placementtype).

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


Représente un objet [ReflectionEffect](../../com.aspose.cells/reflectioneffect) qui spécifie l'effet de réflexion pour l'élément de graphique ou la forme.

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


Indique si la forme est relative à la taille de l'image originale.

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


Conversion du SmartArt en formes groupées.

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


Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte.

**Example**

```
         FontSetting[] list = shape.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - Tous les objets Characters
### getRight() {#getRight--}
```
public int getRight()
```


Représente la largeur du décalage horizontal de la forme par rapport à la colonne de son coin inférieur droit, en unité de pixels.

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


Obtient la rotation de la forme.

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


Représente un objet [ShadowEffect](../../com.aspose.cells/shadoweffect) qui spécifie l'effet d'ombre pour l'élément de graphique ou la forme.

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


Obtient le rayon du flou à appliquer aux bords, en unité de points.

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


Spécifie un identifiant de chaîne optionnel qu’une application peut utiliser pour identifier la forme particulière.

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


Spécifie un nombre optionnel qu’une application peut utiliser pour associer la forme particulière à un type de forme défini.

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


Obtient le texte de cette forme.

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


Obtient le paramètre du texte de la forme.

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


Obtient les informations de texte dans la forme

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


Obtient la direction du flux de texte pour cet objet.

Voir [TextDirectionType](../../com.aspose.cells/textdirectiontype).

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


Renvoie un objet TextEffectFormat qui contient les propriétés de formatage d'effet de texte pour la forme spécifiée. S'applique aux objets Shape qui représentent du WordArt.

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


Obtient le type d’alignement horizontal du texte de la forme.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Obtient le type de dépassement horizontal du texte de la forme qui contient du texte.

Voir [TextOverflowType](../../com.aspose.cells/textoverflowtype).

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


Représente les options de texte de la forme.

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


Obtient le type d’orientation du texte de la forme.

Voir [TextOrientationType](../../com.aspose.cells/textorientationtype).

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


Obtient le type de forme texte prédéfini.

Voir [AutoShapeType](../../com.aspose.cells/autoshapetype).

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


Obtient le type d’alignement vertical du texte de la forme.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Obtient le type de dépassement vertical du texte de la forme qui contient du texte.

Voir [TextOverflowType](../../com.aspose.cells/textoverflowtype).

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


Obtient le format 3D de la forme.

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


Spécifie le titre (légende) de l’objet forme actuel.

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


Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pixels.

**Remarks**

Si la forme se trouve dans le graphique, représente le décalage vertical de la forme par rapport à sa bordure supérieure.

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


Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de centimètres.

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


Représente le décalage vertical de la forme depuis la bordure supérieure de la forme parent, en unité de 1/4000 de la hauteur de la forme parent.

**Remarks**

S'applique uniquement lorsque cette forme se trouve dans le groupe ou le graphique.

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


Représente le décalage vertical de la forme depuis sa ligne supérieure, en unité de pouces.

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


Obtient le décalage vertical de la forme depuis la bordure supérieure de la feuille de calcul, en unité de pixels.

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


Obtient le type de forme automatique.

Voir [AutoShapeType](../../com.aspose.cells/autoshapetype).

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


Obtient le décalage horizontal de la forme depuis la colonne de son coin supérieur gauche.

**Remarks**

La plage de valeurs est de 0 à 1024.

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


Obtient le décalage vertical de la forme depuis la ligne de son coin supérieur gauche.

**Remarks**

La plage de valeurs est de 0 à 256.

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


Représente l’indice de colonne du coin supérieur gauche.

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


Représente l'index de la ligne supérieure.

**Remarks**

Si la forme est dans une forme ou dans un groupe, UpperLeftRow sera ignoré.

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


Représente la largeur de la forme, en unités de pixels.

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


Représente la largeur de la forme, en unités de centimètres.

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


Représente la largeur de la forme, en unités de 1/4000 de la forme parente.

**Remarks**

S'applique uniquement lorsque cette forme se trouve dans le groupe ou le graphique.

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


Représente la largeur de la forme, en unités de pouce.

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


Représente la largeur de la forme, en unités de point.

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


Obtient l'échelle de largeur, en pourcentage de la largeur originale de l'image. Si la forme n'est pas une image, la propriété WidthScale ne renvoie que 100 ;

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


Obtient l'objet [Worksheet](../../com.aspose.cells/worksheet) qui contient cette forme.

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


Obtient le décalage horizontal de la forme par rapport à la bordure gauche de la feuille de calcul, en unités de pixels.

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


Obtient le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul, en unités de pixels.

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


Renvoie la position d'une forme dans l'ordre Z.

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


Obtient la visibilité de la bordure de ligne de la forme.

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


Vrai signifie que le rapport d'aspect de la forme est verrouillé.

**Remarks**

Uniquement pour les images et les objets Ole.

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


Indique si l'objet est décoratif.

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


Indique si la forme ne contient qu'une équation.

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


Indique si le format de remplissage est visible.

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


Obtient si la forme est retournée horizontalement.

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


Obtient si la forme est retournée verticalement.

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


Indique si cette forme est une forme groupée.

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


Indique si l'objet est visible.

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


Indique si la forme est groupée.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


Vrai signifie que le rapport d'aspect de la forme est verrouillé.

**Remarks**

Uniquement pour les images et les objets Ole. NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.IsAspectRatioLocked. Cette propriété sera supprimée 12 mois plus tard à compter de juillet 2024. Aspose s’excuse pour tout inconvénient que vous auriez pu rencontrer.

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


True signifie que l'objet ne peut pas être modifié lorsque la feuille est protégée. Notez que cette valeur n'est pertinente que si la feuille de calcul ou les objets dans la feuille de calcul sont protégés.

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


Indique si l'objet est imprimable. Si False, cette forme ne sera pas imprimée lors de l'impression.

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


Indique si le texte est du texte enrichi.

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


Renvoie si la forme est identique.

**Example**

```
         if (shape.isSameSetting(shape))
             System.out.println("Two objects the same.");
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### isSmartArt() {#isSmartArt--}
```
public boolean isSmartArt()
```


Indique si la forme est un SmartArt.

**Remarks**

Uniquement pour le fichier ooxml.

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


Obtient le type d'habillage du texte de la forme qui contient du texte.

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


Indique si cette forme est un WordArt.

**Remarks**

Uniquement pour la forme Legacy du fichier xls.

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


Déplace la forme vers une plage spécifiée.

**Example**

```
         shape.moveToRange(12, 3, 13, 5);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| bottomRow | int | Indice de ligne en bas à droite |
| rightColumn | int | Indice de colonne en bas à droite |

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


Supprime le contrôle ActiveX.

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


Supprime le lien hypertexte de la forme.

**Example**

```
         shape.removeHyperlink();
```

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Renvoie ou définit la chaîne de texte descriptive (alternative) de l'objet [Shape](../../com.aspose.cells/shape).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setAnchorType(int value) {#setAnchorType-int-}
```
public void setAnchorType(int value)
```


Définit le type de l'espace réservé d'ancrage de la forme.

Voir [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setAspectRatioLocked(boolean value) {#setAspectRatioLocked-boolean-}
```
public void setAspectRatioLocked(boolean value)
```


Vrai signifie que le rapport d'aspect de la forme est verrouillé.

**Remarks**

Uniquement pour les images et les objets Ole.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutoShapeType(int value) {#setAutoShapeType-int-}
```
public void setAutoShapeType(int value)
```


Définit le type de forme automatique.

Voir [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


Représente la largeur du décalage vertical de la forme depuis la rangée de son coin inférieur, en unités de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCreateId(UUID value) {#setCreateId-java.util.UUID-}
```
public void setCreateId(UUID value)
```


Définit l'ID de création pour cette forme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.UUID |  |

### setDecorative(boolean value) {#setDecorative-boolean-}
```
public void setDecorative(boolean value)
```


Indique si l'objet est décoratif.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFilled(boolean value) {#setFilled-boolean-}
```
public void setFilled(boolean value)
```


Indique si le format de remplissage est visible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFlippedHorizontally(boolean value) {#setFlippedHorizontally-boolean-}
```
public void setFlippedHorizontally(boolean value)
```


Définit si la forme est retournée horizontalement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


Définit si la forme est retournée verticalement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFont(Font value) {#setFont-com.aspose.cells.Font-}
```
public void setFont(Font value)
```


Représente la police de la forme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Font](../../com.aspose.cells/font) |  |

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


Représente la hauteur de la forme, en unité de centimètres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setHeightInShape(int value) {#setHeightInShape-int-}
```
public void setHeightInShape(int value)
```


Représente le décalage vertical de la forme depuis la bordure supérieure de la forme parente, en unité de 1/4000 de la hauteur de la forme parente.

**Remarks**

S'applique uniquement lorsque cette forme se trouve dans le groupe ou le graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

### setInputRange(String value) {#setInputRange-java.lang.String-}
```
public void setInputRange(String value)
```


Définit la plage de feuille de calcul utilisée pour remplir la zone combinée spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setInputRange(String formula, boolean isR1C1, boolean isLocal) {#setInputRange-java.lang.String-boolean-boolean-}
```
public void setInputRange(String formula, boolean isR1C1, boolean isLocal)
```


Définit la plage utilisée pour remplir le contrôle.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | La plage utilisée pour remplir le contrôle. |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |

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

### setLeftInShape(int value) {#setLeftInShape-int-}
```
public void setLeftInShape(int value)
```


Représente le décalage horizontal de la forme par rapport à la bordure gauche de la forme parent, en unité de 1/4000 de la largeur de la forme parent.

**Remarks**

S'applique uniquement lorsque cette forme se trouve dans le groupe ou le graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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


Définit le décalage horizontal de la forme par rapport à la bordure gauche de la feuille de calcul.

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

### setLinkedCell(String formula, boolean isR1C1, boolean isLocal) {#setLinkedCell-java.lang.String-boolean-boolean-}
```
public void setLinkedCell(String formula, boolean isR1C1, boolean isLocal)
```


Définit la plage liée à la valeur du contrôle.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | La plage liée à la valeur du contrôle. |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


Vrai signifie que le rapport d'aspect de la forme est verrouillé.

**Remarks**

Uniquement pour les images et les objets Ole. NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.IsAspectRatioLocked. Cette propriété sera supprimée 12 mois plus tard à compter de juillet 2024. Aspose s’excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


True signifie que l'objet ne peut pas être modifié lorsque la feuille est protégée. Notez que cette valeur n'est pertinente que si la feuille de calcul ou les objets dans la feuille de calcul sont protégés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLockedProperty(int type, boolean value) {#setLockedProperty-int-boolean-}
```
public void setLockedProperty(int type, boolean value)
```


Définit la propriété verrouillée.

**Example**

```
         shape.setLockedProperty(ShapeLockType.ADJUST_HANDLES, true);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). Le type verrouillé. |
| valeur | boolean | La valeur de la propriété. |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


Définit le décalage horizontal de la forme depuis la colonne de son coin inférieur droit.

**Remarks**

La plage de valeurs est de 0 à 1024.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


Définit le décalage vertical de la forme depuis la ligne de son coin inférieur droit.

**Remarks**

La plage de valeurs est de 0 à 256.

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

### setMacroName(String value) {#setMacroName-java.lang.String-}
```
public void setMacroName(String value)
```


Définit le nom de la macro.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Définit le nom de la forme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Représente la façon dont l'objet de dessin est attaché aux cellules en dessous. La propriété contrôle le placement d'un objet sur une feuille de calcul.

Voir [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


Indique si l'objet est imprimable. Si False, cette forme ne sera pas imprimée lors de l'impression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

### setSoftEdges(double value) {#setSoftEdges-double-}
```
public void setSoftEdges(double value)
```


Définit le rayon du flou à appliquer aux bords, en unité de points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Définit le texte de cette forme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Définit la direction du flux de texte pour cet objet.

Voir [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Définit le type d'alignement horizontal du texte de la forme.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Définit le type de débordement horizontal du texte de la forme contenant du texte.

Voir [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextOptions(TextOptions value) {#setTextOptions-com.aspose.cells.TextOptions-}
```
public void setTextOptions(TextOptions value)
```


Représente les options de texte de la forme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [TextOptions](../../com.aspose.cells/textoptions) |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


Définit le type d'orientation du texte de la forme.

Voir [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Définit le type de forme texte prédéfini.

Voir [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Définit le type d'alignement vertical du texte de la forme.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Définit le type de débordement vertical du texte de la forme contenant du texte.

Voir [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

### setTopInShape(int value) {#setTopInShape-int-}
```
public void setTopInShape(int value)
```


Représente le décalage vertical de la forme depuis la bordure supérieure de la forme parent, en unité de 1/4000 de la hauteur de la forme parent.

**Remarks**

S'applique uniquement lorsque cette forme se trouve dans le groupe ou le graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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


Définit le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul, en unité de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


Définit le décalage horizontal de la forme par rapport à la colonne de son coin supérieur gauche.

**Remarks**

La plage de valeurs est de 0 à 1024.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


Définit le décalage vertical de la forme par rapport à la ligne de son coin supérieur gauche.

**Remarks**

La plage de valeurs est de 0 à 256.

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


Représente l'index de la ligne supérieure.

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

### setWidthInShape(int value) {#setWidthInShape-int-}
```
public void setWidthInShape(int value)
```


Représente la largeur de la forme, en unités de 1/4000 de la forme parente.

**Remarks**

S'applique uniquement lorsque cette forme se trouve dans le groupe ou le graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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


Définit le décalage horizontal de la forme par rapport à la bordure gauche de la feuille de calcul, en unité de pixels.

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

### toFrontOrBack(int orders) {#toFrontOrBack-int-}
```
public void toFrontOrBack(int orders)
```


Place la forme au premier plan ou l'envoie à l'arrière-plan.

**Example**

```
         shape.toFrontOrBack(2);
         //or shape.ToFrontOrBack(-1);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| orders | int | Si c'est inférieur à zéro, place la forme à l'arrière. Si c'est supérieur à zéro, amène la forme au premier plan. |

### toImage(OutputStream stream, ImageFormat imageFormat) {#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-}
```
public void toImage(OutputStream stream, ImageFormat imageFormat)
```


Crée l'image de la forme et l'enregistre dans un flux au format spécifié.

**Remarks**

Les formats suivants sont pris en charge : .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux de sortie. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | Le format dans lequel enregistrer l'image. |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Enregistre la forme dans un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


Enregistre la forme dans un fichier.

**Example**

```
         ImageOrPrintOptions op = new ImageOrPrintOptions();
         shape.toImage("exmaple.png", op);
```

**Parameters:**
| Paramètre | Type | Description |
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


Met à jour la valeur sélectionnée avec la valeur de la cellule liée.

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

