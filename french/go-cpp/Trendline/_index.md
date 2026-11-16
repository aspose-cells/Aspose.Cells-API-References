---
title: "Classe Trendline"
linktitle: "Trendline"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe Trendline. Encapsule l'objet qui représente trendline en Go."
type: docs
weight: 200
url: /fr/go-cpp/trendline/
---

## Trendline class

Représente une ligne de tendance dans un graphique.

```go

type Trendline struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewTrendline](./newtrendline/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [IsNameAuto](./isnameauto/) | Renvoie si Microsoft Excel détermine automatiquement le nom de la courbe de tendance. |
| [SetIsNameAuto](./setisnameauto/) | Renvoie si Microsoft Excel détermine automatiquement le nom de la courbe de tendance. |
| [GetType](./gettype/) | Renvoie le type de la courbe de tendance. |
| [GetName](./getname/) | Renvoie le nom de la courbe de tendance. |
| [SetName](./setname/) | Renvoie le nom de la courbe de tendance. |
| [GetOrder](./getorder/) | Renvoie ou définit l'ordre de la courbe de tendance (un entier supérieur à 1) lorsque le type de courbe de tendance est Polynomial. L'ordre doit être compris entre 2 et 6. |
| [SetOrder](./setorder/) | Renvoie ou définit l'ordre de la courbe de tendance (un entier supérieur à 1) lorsque le type de courbe de tendance est Polynomial. L'ordre doit être compris entre 2 et 6. |
| [GetPeriod](./getperiod/) | Renvoie ou définit la période pour la courbe de tendance moyenne mobile. |
| [SetPeriod](./setperiod/) | Renvoie ou définit la période pour la courbe de tendance moyenne mobile. |
| [GetForward](./getforward/) | Renvoie ou définit le nombre de périodes (ou d'unités sur un graphique de dispersion) que la courbe de tendance étend vers l'avant. Le nombre de périodes doit être supérieur ou égal à zéro. |
| [SetForward](./setforward/) | Renvoie ou définit le nombre de périodes (ou d'unités sur un graphique de dispersion) que la courbe de tendance étend vers l'avant. Le nombre de périodes doit être supérieur ou égal à zéro. |
| [GetBackward](./getbackward/) | Renvoie ou définit le nombre de périodes (ou d'unités sur un graphique de dispersion) que la courbe de tendance étend vers l'arrière. Le nombre de périodes doit être supérieur ou égal à zéro. Si le type de graphique est en colonnes, le nombre de périodes doit être compris entre 0 et 0,5. |
| [SetBackward](./setbackward/) | Renvoie ou définit le nombre de périodes (ou d'unités sur un graphique de dispersion) que la courbe de tendance étend vers l'arrière. Le nombre de périodes doit être supérieur ou égal à zéro. Si le type de graphique est en colonnes, le nombre de périodes doit être compris entre 0 et 0,5. |
| [GetDisplayEquation](./getdisplayequation/) | Indique si l'équation de la courbe de tendance est affichée sur le graphique (dans la même étiquette de données que la valeur R-carré). Définir cette propriété sur True active automatiquement les étiquettes de données. |
| [SetDisplayEquation](./setdisplayequation/) | Indique si l'équation de la courbe de tendance est affichée sur le graphique (dans la même étiquette de données que la valeur R-carré). Définir cette propriété sur True active automatiquement les étiquettes de données. |
| [GetDisplayRSquared](./getdisplayrsquared/) | Indique si la valeur R-carré de la courbe de tendance est affichée sur le graphique (dans la même étiquette de données que l'équation). Définir cette propriété sur True active automatiquement les étiquettes de données. |
| [SetDisplayRSquared](./setdisplayrsquared/) | Indique si la valeur R-carré de la courbe de tendance est affichée sur le graphique (dans la même étiquette de données que l'équation). Définir cette propriété sur True active automatiquement les étiquettes de données. |
| [GetIntercept](./getintercept/) | Renvoie ou définit le point où la courbe de tendance croise l'axe des valeurs. |
| [SetIntercept](./setintercept/) | Renvoie ou définit le point où la courbe de tendance croise l'axe des valeurs. |
| [GetDataLabels](./getdatalabels/) | Représente l'objet DataLabels pour la série spécifiée. |
| [GetLegendEntry](./getlegendentry/) | Obtient l'entrée de légende correspondant à cette courbe de tendance |
| [GetCompoundType](./getcompoundtype/) | Spécifie le type de ligne composée |
| [SetCompoundType](./setcompoundtype/) | Spécifie le type de ligne composée |
| [GetDashType](./getdashtype/) | Spécifie le type de ligne pointillée |
| [SetDashType](./setdashtype/) | Spécifie le type de ligne pointillée |
| [GetCapType](./getcaptype/) | Spécifie les extrémités finales. |
| [SetCapType](./setcaptype/) | Spécifie les extrémités finales. |
| [GetJoinType](./getjointype/) | Spécifie les extrémités de jointure. |
| [SetJoinType](./setjointype/) | Spécifie les extrémités de jointure. |
| [GetBeginType](./getbegintype/) | Spécifie une pointe de flèche pour le début d'une ligne. |
| [SetBeginType](./setbegintype/) | Spécifie une pointe de flèche pour le début d'une ligne. |
| [GetEndType](./getendtype/) | Spécifie une pointe de flèche pour la fin d'une ligne. |
| [SetEndType](./setendtype/) | Spécifie une pointe de flèche pour la fin d'une ligne. |
| [GetBeginArrowLength](./getbeginarrowlength/) | Spécifie la longueur de la pointe de flèche pour le début d'une ligne. |
| [SetBeginArrowLength](./setbeginarrowlength/) | Spécifie la longueur de la pointe de flèche pour le début d'une ligne. |
| [GetEndArrowLength](./getendarrowlength/) | Spécifie la longueur de la pointe de flèche pour la fin d'une ligne. |
| [SetEndArrowLength](./setendarrowlength/) | Spécifie la longueur de la pointe de flèche pour la fin d'une ligne. |
| [GetBeginArrowWidth](./getbeginarrowwidth/) | Spécifie la largeur de la pointe de flèche pour le début d'une ligne. |
| [SetBeginArrowWidth](./setbeginarrowwidth/) | Spécifie la largeur de la pointe de flèche pour le début d'une ligne. |
| [GetEndArrowWidth](./getendarrowwidth/) | Spécifie la largeur de la pointe de flèche pour la fin d'une ligne. |
| [SetEndArrowWidth](./setendarrowwidth/) | Spécifie la largeur de la pointe de flèche pour la fin d'une ligne. |
| [GetThemeColor](./getthemecolor/) | Obtient et définit la couleur du thème. |
| [SetThemeColor](./setthemecolor/) | Obtient et définit la couleur du thème. |
| [GetColor](./getcolor/) | Représente la couleur de la ligne. |
| [SetColor](./setcolor/) | Représente la couleur de la ligne. |
| [GetTransparency](./gettransparency/) | Renvoie ou définit le degré de transparence de la ligne sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent). |
| [SetTransparency](./settransparency/) | Renvoie ou définit le degré de transparence de la ligne sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent). |
| [GetStyle](./getstyle/) | Représente le style de la ligne. |
| [SetStyle](./setstyle/) | Représente le style de la ligne. |
| [GetWeight](./getweight/) | Obtient ou définit le WeightType de la ligne. |
| [SetWeight](./setweight/) | Obtient ou définit le WeightType de la ligne. |
| [GetWeightPt](./getweightpt/) | Obtient ou définit le poids de la ligne en points. |
| [SetWeightPt](./setweightpt/) | Obtient ou définit le poids de la ligne en points. |
| [GetWeightPx](./getweightpx/) | Obtient ou définit le poids de la ligne en pixels. |
| [SetWeightPx](./setweightpx/) | Obtient ou définit le poids de la ligne en pixels. |
| [GetFormattingType](./getformattingtype/) | Obtient ou définit le type de format. |
| [SetFormattingType](./setformattingtype/) | Obtient ou définit le type de format. |
| [IsAutomaticColor](./isautomaticcolor/) | Indique si la couleur de la ligne est attribuée automatiquement. |
| [IsVisible](./isvisible/) | Représente si la ligne est visible. |
| [SetIsVisible](./setisvisible/) | Représente si la ligne est visible. |
| [IsAuto](./isauto/) | Indique si ce style de ligne est attribué automatiquement. |
| [SetIsAuto](./setisauto/) | Indique si ce style de ligne est attribué automatiquement. |
| [GetGradientFill](./getgradientfill/) | Représente le remplissage en dégradé. |
