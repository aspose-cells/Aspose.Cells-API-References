---
title: "Classe Title"
linktitle: "Titre"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe Title. Encapsule l'objet qui représente le titre dans Go."
type: docs
weight: 200
url: /fr/go-cpp/title/
---

## Title class

Encapsule l'objet qui représente le titre d'un graphique ou d'un axe.

```go

type Title struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewTitle](./newtitle/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetText](./gettext/) | Obtient ou définit le texte de l'étiquette de l'unité d'affichage. |
| [SetText](./settext/) | Obtient ou définit le texte de l'étiquette de l'unité d'affichage. |
| [IsVisible](./isvisible/) | Indique si le titre est visible. |
| [SetIsVisible](./setisvisible/) | Indique si le titre est visible. |
| [GetXRatioToChart](./getxratiotochart/) | Obtient ou définit la coordonnée x du coin supérieur gauche en unités de Fraction de la zone du graphique. X en pixels = XRatioToChart * Chart.ChartObject.Width; |
| [SetXRatioToChart](./setxratiotochart/) | Obtient ou définit la coordonnée x du coin supérieur gauche en unités de Fraction de la zone du graphique. X en pixels = XRatioToChart * Chart.ChartObject.Width; |
| [GetYRatioToChart](./getyratiotochart/) | Obtient ou définit la coordonnée y du coin supérieur gauche en unités de Fraction de la zone du graphique. Y en pixels = YRatioToChart * Chart.ChartObject.Width; |
| [SetYRatioToChart](./setyratiotochart/) | Obtient ou définit la coordonnée y du coin supérieur gauche en unités de Fraction de la zone du graphique. Y en pixels = YRatioToChart * Chart.ChartObject.Width; |
| [GetOverLay](./getoverlay/) | Représente un titre superposé centré sur un graphique sans redimensionner le graphique. |
| [SetOverLay](./setoverlay/) | Représente un titre superposé centré sur un graphique sans redimensionner le graphique. |
| [Characters](./characters/) | Obtient le formatage du texte enrichi de ce Title. |
| [Characters_Int_Int](./characters_int_int/) | Renvoie un objet Characters qui représente une plage de caractères dans le texte. |
| [IsInnerMode](./isinnermode/) | Indique si la taille de la zone de tracé inclut les marques de graduation et les étiquettes d'axe. False spécifie que la taille doit déterminer la taille de la zone de tracé, les marques de graduation et les étiquettes d'axe. |
| [SetIsInnerMode](./setisinnermode/) | Indique si la taille de la zone de tracé inclut les marques de graduation et les étiquettes d'axe. False spécifie que la taille doit déterminer la taille de la zone de tracé, les marques de graduation et les étiquettes d'axe. |
| [GetShadow](./getshadow/) | True si le cadre possède une ombre. |
| [SetShadow](./setshadow/) | True si le cadre possède une ombre. |
| [GetShapeProperties](./getshapeproperties/) | Obtient l'objet ShapeProperties. |
| [IsDefaultPosBeSet](./isdefaultposbeset/) | Indique si la position par défaut (DefaultX, DefaultY, DefaultWidth et DefaultHeight) est définie. |
| [GetDefaultXRatioToChart](./getdefaultxratiotochart/) | Représente x de la position par défaut en unités de Fraction de la zone du graphique. |
| [GetDefaultYRatioToChart](./getdefaultyratiotochart/) | Représente y de la position par défaut en unités de la fraction de la zone du graphique. |
| [GetDefaultWidthRatioToChart](./getdefaultwidthratiotochart/) | Représente la largeur de la position par défaut en unités de Fraction de la zone du graphique. |
| [GetDefaultHeightRatioToChart](./getdefaultheightratiotochart/) | Représente la hauteur de la position par défaut en unités de la fraction de la zone du graphique. |
| [GetBorder](./getborder/) | Obtient le Line</see>. |
| [GetArea](./getarea/) | Obtient le Area</see>. |
| [GetTextOptions](./gettextoptions/) | Obtient et définit les options du texte. |
| [GetFont](./getfont/) | Obtient un objet Font de l'objet ChartFrame spécifié. |
| [GetAutoScaleFont](./getautoscalefont/) | True si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est True. |
| [SetAutoScaleFont](./setautoscalefont/) | True si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est True. |
| [IsAutomaticSize](./isautomaticsize/) | Indique si le cadre du graphique est dimensionné automatiquement. |
| [SetIsAutomaticSize](./setisautomaticsize/) | Indique si le cadre du graphique est dimensionné automatiquement. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | Obtient ou définit la largeur du cadre en unités du rapport de la zone du graphique. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | Obtient ou définit la largeur du cadre en unités du rapport de la zone du graphique. |
| [GetHeightRatioToChart](./getheightratiotochart/) | Obtient ou définit la hauteur du cadre en unités du rapport de la zone du graphique. |
| [SetHeightRatioToChart](./setheightratiotochart/) | Obtient ou définit la hauteur du cadre en unités du rapport de la zone du graphique. |
| [GetXPixel](./getxpixel/) | Obtient ou définit la coordonnée x du coin supérieur gauche en unités de Pixel. |
| [SetXPixel](./setxpixel/) | Obtient ou définit la coordonnée x du coin supérieur gauche en unités de Pixel. |
| [GetYPixel](./getypixel/) | Obtient ou définit la coordonnée y du coin supérieur gauche en unités de pixels. |
| [SetYPixel](./setypixel/) | Obtient ou définit la coordonnée y du coin supérieur gauche en unités de pixels. |
| [GetWidthPixel](./getwidthpixel/) | Obtient ou définit la largeur du cadre en unités de Pixel. |
| [SetWidthPixel](./setwidthpixel/) | Obtient ou définit la largeur du cadre en unités de Pixel. |
| [GetHeightPixel](./getheightpixel/) | Obtient ou définit la hauteur du cadre en unités de pixels. |
| [SetHeightPixel](./setheightpixel/) | Obtient ou définit la hauteur du cadre en unités de pixels. |
| [SetPositionAuto](./setpositionauto/) | Définir la position du cadre sur automatique |
| [IsDeleted](./isdeleted/) | Indique si cette étiquette de données est supprimée. |
| [SetIsDeleted](./setisdeleted/) | Indique si cette étiquette de données est supprimée. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Obtient et définit l'alignement horizontal du texte. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Obtient et définit l'alignement horizontal du texte. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Obtient ou définit l'alignement vertical du texte. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Obtient ou définit l'alignement vertical du texte. |
| [GetRotationAngle](./getrotationangle/) | Représente l'angle de rotation du texte. |
| [SetRotationAngle](./setrotationangle/) | Représente l'angle de rotation du texte. |
| [IsAutomaticRotation](./isautomaticrotation/) | Indique si le texte du graphique est automatiquement tourné. |
| [GetReadingOrder](./getreadingorder/) | Représente l'ordre de lecture du texte. |
| [SetReadingOrder](./setreadingorder/) | Représente l'ordre de lecture du texte. |
| [IsResizeShapeToFitText](./isresizeshapetofittext/) | Obtient ou définit si une forme doit être ajustée automatiquement pour contenir entièrement le texte qui y est décrit. L'ajustement automatique consiste à mettre à l'échelle le texte à l'intérieur d'une forme afin de contenir tout le texte. |
| [SetIsResizeShapeToFitText](./setisresizeshapetofittext/) | Obtient ou définit si une forme doit être ajustée automatiquement pour contenir entièrement le texte qui y est décrit. L'ajustement automatique consiste à mettre à l'échelle le texte à l'intérieur d'une forme afin de contenir tout le texte. |
| [IsAutoText](./isautotext/) | Indique que le texte est généré automatiquement. |
| [SetIsAutoText](./setisautotext/) | Indique que le texte est généré automatiquement. |
| [GetLinkedSource](./getlinkedsource/) | Obtient et définit une référence à la feuille de calcul. |
| [SetLinkedSource](./setlinkedsource/) | Obtient et définit une référence à la feuille de calcul. |
| [GetDirectionType](./getdirectiontype/) | Obtient ou définit la direction du texte. |
| [SetDirectionType](./setdirectiontype/) | Obtient ou définit la direction du texte. |
| [IsTextWrapped](./istextwrapped/) | Obtient ou définit une valeur indiquant si le texte est renvoyé à la ligne. |
| [SetIsTextWrapped](./setistextwrapped/) | Obtient ou définit une valeur indiquant si le texte est renvoyé à la ligne. |
