---
title: "Classe LineFormat"
linktitle: "LineFormat"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe LineFormat. Encapsule l'objet qui représente le lineformat en Go."
type: docs
weight: 200
url: /fr/go-cpp/lineformat/
---

## LineFormat class

Représente tous les paramètres de la ligne.

```go

type LineFormat struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewLineFormat](./newlineformat/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetHashCode](./gethashcode/) | Obtient le code de hachage. |
| [Equals](./equals/) | Détermine si cette instance a la même valeur qu'un autre objet LineFormat spécifié. |
| [GetCompoundType](./getcompoundtype/) | Spécifie le type de composition de la ligne. |
| [SetCompoundType](./setcompoundtype/) | Spécifie le type de composition de la ligne. |
| [GetDashStyle](./getdashstyle/) | Spécifie le type de tiret de la ligne. |
| [SetDashStyle](./setdashstyle/) | Spécifie le type de tiret de la ligne. |
| [GetCapType](./getcaptype/) | Spécifie les extrémités finales. |
| [SetCapType](./setcaptype/) | Spécifie les extrémités finales. |
| [GetJoinType](./getjointype/) | Spécifie le type de jointure de la ligne. |
| [SetJoinType](./setjointype/) | Spécifie le type de jointure de la ligne. |
| [GetBeginArrowheadStyle](./getbeginarrowheadstyle/) | Obtient et définit le type de flèche de début de la ligne. |
| [SetBeginArrowheadStyle](./setbeginarrowheadstyle/) | Obtient et définit le type de flèche de début de la ligne. |
| [GetBeginArrowheadWidth](./getbeginarrowheadwidth/) | Obtient et définit le type de largeur de flèche de début de la ligne. |
| [SetBeginArrowheadWidth](./setbeginarrowheadwidth/) | Obtient et définit le type de largeur de flèche de début de la ligne. |
| [GetBeginArrowheadLength](./getbeginarrowheadlength/) | Obtient et définit le type de longueur de flèche de début de la ligne. |
| [SetBeginArrowheadLength](./setbeginarrowheadlength/) | Obtient et définit le type de longueur de flèche de début de la ligne. |
| [GetEndArrowheadStyle](./getendarrowheadstyle/) | Obtient et définit le type de flèche de fin de la ligne. |
| [SetEndArrowheadStyle](./setendarrowheadstyle/) | Obtient et définit le type de flèche de fin de la ligne. |
| [GetEndArrowheadWidth](./getendarrowheadwidth/) | Obtient et définit le type de largeur de flèche de fin de la ligne. |
| [SetEndArrowheadWidth](./setendarrowheadwidth/) | Obtient et définit le type de largeur de flèche de fin de la ligne. |
| [GetEndArrowheadLength](./getendarrowheadlength/) | Obtient et définit le type de longueur de flèche de fin de la ligne. |
| [SetEndArrowheadLength](./setendarrowheadlength/) | Obtient et définit le type de longueur de flèche de fin de la ligne. |
| [GetWeight](./getweight/) | Obtient ou définit le poids de la ligne en points. |
| [SetWeight](./setweight/) | Obtient ou définit le poids de la ligne en points. |
| [GetFillType](./getfilltype/) | Obtient et définit le type de remplissage |
| [SetFillType](./setfilltype/) | Obtient et définit le type de remplissage |
| [GetTransparency](./gettransparency/) | Renvoie ou définit le degré de transparence de la zone sous forme d'une valeur allant de 0,0 (opaque) à 1,0 (transparent). |
| [SetTransparency](./settransparency/) | Renvoie ou définit le degré de transparence de la zone sous forme d'une valeur allant de 0,0 (opaque) à 1,0 (transparent). |
| [GetGradientFill](./getgradientfill/) | Obtient l'objet GradientFill. |
| [GetTextureFill](./gettexturefill/) | Obtient l'objet TextureFill. |
| [GetSolidFill](./getsolidfill/) | Obtient l'objet SolidFill. |
| [GetPatternFill](./getpatternfill/) | Obtient l'objet PatternFill. |
| [GetGradientColorType](./getgradientcolortype/) | Renvoie le type de couleur du dégradé pour le remplissage spécifié. |
| [GetGradientStyle](./getgradientstyle/) | Renvoie le style du dégradé pour le remplissage spécifié. |
| [GetGradientColor1](./getgradientcolor1/) | Renvoie la couleur 1 du dégradé pour le remplissage spécifié. |
| [GetGradientColor2](./getgradientcolor2/) | Renvoie la couleur 2 du dégradé pour le remplissage spécifié. |
| [GetGradientDegree](./getgradientdegree/) | Renvoie le degré du dégradé pour le remplissage spécifié. S'applique uniquement à Excel 2007. |
| [GetGradientVariant](./getgradientvariant/) | Renvoie la variante du dégradé pour le remplissage spécifié. S'applique uniquement à Excel 2007. |
| [GetPresetColor](./getpresetcolor/) | Renvoie la couleur de dégradé prédéfinie pour le remplissage spécifié. |
| [SetOneColorGradient](./setonecolorgradient/) | Définit le remplissage spécifié en un dégradé à une couleur. S'applique uniquement à Excel 2007. |
| [SetTwoColorGradient_Color_Color_GradientStyleType_Int](./settwocolorgradient_color_color_gradientstyletype_int/) | Définit le remplissage spécifié en un dégradé à deux couleurs. S'applique uniquement à Excel 2007. |
| [SetPresetColorGradient](./setpresetcolorgradient/) | Définit le remplissage spécifié avec un dégradé de couleur prédéfinie. S'applique uniquement à Excel 2007. |
| [GetTexture](./gettexture/) | Représente le type de texture pour le remplissage spécifié. |
| [SetTexture](./settexture/) | Représente le type de texture pour le remplissage spécifié. |
| [GetPattern](./getpattern/) | Représente le motif d'affichage d'une zone. |
| [SetPattern](./setpattern/) | Représente le motif d'affichage d'une zone. |
| [GetPictureFormatType](./getpictureformattype/) | Obtient et définit le type de format d'image. |
| [SetPictureFormatType](./setpictureformattype/) | Obtient et définit le type de format d'image. |
| [GetScale](./getscale/) | Obtient et définit l'échelle du format d'image. |
| [SetScale](./setscale/) | Obtient et définit l'échelle du format d'image. |
| [GetImageData](./getimagedata/) | Obtient et définit les données d'image de la photo. |
| [SetImageData](./setimagedata/) | Obtient et définit les données d'image de la photo. |
