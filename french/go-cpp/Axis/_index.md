---
title: "Classe Axis"
linktitle: "Axis"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe Axis. Encapsule l'objet qui représente l'axe dans Go."
type: docs
weight: 200
url: /fr/go-cpp/axis/
---

## Axis class

Encapsule l'objet qui représente un axe d'un graphique.

```go

type Axis struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetArea](./getarea/) | Obtient la zone. |
| [IsAutomaticMinValue](./isautomaticminvalue/) | Indique si la valeur minimale est attribuée automatiquement. |
| [SetIsAutomaticMinValue](./setisautomaticminvalue/) | Indique si la valeur minimale est attribuée automatiquement. |
| [GetMinValue](./getminvalue/) | Représente la valeur minimale sur l'axe des valeurs. |
| [SetMinValue](./setminvalue/) | Représente la valeur minimale sur l'axe des valeurs. |
| [IsAutomaticMaxValue](./isautomaticmaxvalue/) | Indique si la valeur maximale est attribuée automatiquement. |
| [SetIsAutomaticMaxValue](./setisautomaticmaxvalue/) | Indique si la valeur maximale est attribuée automatiquement. |
| [GetMaxValue](./getmaxvalue/) | Représente la valeur maximale sur l'axe des valeurs. |
| [SetMaxValue](./setmaxvalue/) | Représente la valeur maximale sur l'axe des valeurs. |
| [IsAutomaticMajorUnit](./isautomaticmajorunit/) | Indique si l'unité principale de l'axe est attribuée automatiquement. |
| [SetIsAutomaticMajorUnit](./setisautomaticmajorunit/) | Indique si l'unité principale de l'axe est attribuée automatiquement. |
| [GetMajorUnit](./getmajorunit/) | Représente les unités principales de l'axe. |
| [SetMajorUnit](./setmajorunit/) | Représente les unités principales de l'axe. |
| [IsAutomaticMinorUnit](./isautomaticminorunit/) | Indique si l'unité secondaire de l'axe est attribuée automatiquement. |
| [SetIsAutomaticMinorUnit](./setisautomaticminorunit/) | Indique si l'unité secondaire de l'axe est attribuée automatiquement. |
| [GetMinorUnit](./getminorunit/) | Représente les unités secondaires de l'axe. |
| [SetMinorUnit](./setminorunit/) | Représente les unités secondaires de l'axe. |
| [GetAxisLine](./getaxisline/) | Obtient l'apparence d'un Axis. |
| [GetMajorTickMark](./getmajortickmark/) | Représente le type de graduation principale pour l'axe spécifié. |
| [SetMajorTickMark](./setmajortickmark/) | Représente le type de graduation principale pour l'axe spécifié. |
| [GetMinorTickMark](./getminortickmark/) | Représente le type de graduation secondaire pour l'axe spécifié. |
| [SetMinorTickMark](./setminortickmark/) | Représente le type de graduation secondaire pour l'axe spécifié. |
| [GetTickLabelPosition](./getticklabelposition/) | Représente la position des étiquettes de graduation sur l'axe spécifié. |
| [SetTickLabelPosition](./setticklabelposition/) | Représente la position des étiquettes de graduation sur l'axe spécifié. |
| [GetCrossAt](./getcrossat/) | Représente le point sur l'axe des valeurs où l'axe des catégories le traverse. |
| [SetCrossAt](./setcrossat/) | Représente le point sur l'axe des valeurs où l'axe des catégories le traverse. |
| [GetCrossType](./getcrosstype/) | Représente le CrossType sur l'axe spécifié où l'autre axe le traverse. |
| [SetCrossType](./setcrosstype/) | Représente le CrossType sur l'axe spécifié où l'autre axe le traverse. |
| [GetLogBase](./getlogbase/) | Représente la base logarithmique. La valeur par défaut est 10. |
| [SetLogBase](./setlogbase/) | Représente la base logarithmique. La valeur par défaut est 10. |
| [IsLogarithmic](./islogarithmic/) | Indique si le type d'échelle de l'axe des valeurs est logarithmique ou non. |
| [SetIsLogarithmic](./setislogarithmic/) | Indique si le type d'échelle de l'axe des valeurs est logarithmique ou non. |
| [IsPlotOrderReversed](./isplotorderreversed/) | Indique si Microsoft Excel trace les points de données du dernier au premier. |
| [SetIsPlotOrderReversed](./setisplotorderreversed/) | Indique si Microsoft Excel trace les points de données du dernier au premier. |
| [GetAxisBetweenCategories](./getaxisbetweencategories/) | Représente si l'axe des valeurs croise l'axe des catégories entre les catégories. |
| [SetAxisBetweenCategories](./setaxisbetweencategories/) | Représente si l'axe des valeurs croise l'axe des catégories entre les catégories. |
| [GetTickLabels](./getticklabels/) | Renvoie un objet TickLabels qui représente les étiquettes des marques de graduation pour l'axe spécifié. |
| [GetTickLabelSpacing](./getticklabelspacing/) | Représente le nombre de catégories ou de séries entre les étiquettes des marques de graduation. S'applique uniquement aux axes de catégorie et de séries. |
| [SetTickLabelSpacing](./setticklabelspacing/) | Représente le nombre de catégories ou de séries entre les étiquettes des marques de graduation. S'applique uniquement aux axes de catégorie et de séries. |
| [IsAutoTickLabelSpacing](./isautoticklabelspacing/) | Indique si l'espacement des étiquettes de graduation est automatique |
| [SetIsAutoTickLabelSpacing](./setisautoticklabelspacing/) | Indique si l'espacement des étiquettes de graduation est automatique |
| [GetTickMarkSpacing](./gettickmarkspacing/) | Renvoie ou définit le nombre de catégories ou de séries entre les marques de graduation. S'applique uniquement aux axes de catégorie et de séries. |
| [SetTickMarkSpacing](./settickmarkspacing/) | Renvoie ou définit le nombre de catégories ou de séries entre les marques de graduation. S'applique uniquement aux axes de catégorie et de séries. |
| [GetDisplayUnit](./getdisplayunit/) | Représente l'étiquette d'unité pour l'axe spécifié. |
| [SetDisplayUnit](./setdisplayunit/) | Représente l'étiquette d'unité pour l'axe spécifié. |
| [GetCustomDisplayUnit](./getcustomdisplayunit/) | Spécifie une valeur personnalisée pour l'unité d'affichage. |
| [SetCustomDisplayUnit](./setcustomdisplayunit/) | Spécifie une valeur personnalisée pour l'unité d'affichage. |
| [GetDisplayUnitLabel](./getdisplayunitlabel/) | Représente une étiquette d'unité sur un axe dans le graphique spécifié. Les étiquettes d'unité sont utiles pour tracer de grandes valeurs - par exemple, en millions ou en milliards. |
| [IsDisplayUnitLabelShown](./isdisplayunitlabelshown/) | Représente si l'étiquette d'unité d'affichage est affichée sur l'axe spécifié. |
| [SetIsDisplayUnitLabelShown](./setisdisplayunitlabelshown/) | Représente si l'étiquette d'unité d'affichage est affichée sur l'axe spécifié. |
| [GetTitle](./gettitle/) | Obtient le titre de cet axe dans le graphique. |
| [GetCategoryType](./getcategorytype/) | Représente le type de l'axe des catégories. |
| [SetCategoryType](./setcategorytype/) | Représente le type de l'axe des catégories. |
| [GetBaseUnitScale](./getbaseunitscale/) | Représente l'échelle de l'unité de base pour l'axe des catégories. |
| [SetBaseUnitScale](./setbaseunitscale/) | Représente l'échelle de l'unité de base pour l'axe des catégories. |
| [GetMajorUnitScale](./getmajorunitscale/) | Représente l'échelle de l'unité principale pour l'axe des catégories. |
| [SetMajorUnitScale](./setmajorunitscale/) | Représente l'échelle de l'unité principale pour l'axe des catégories. |
| [GetMinorUnitScale](./getminorunitscale/) | Représente l'échelle de l'unité principale pour l'axe des catégories. |
| [SetMinorUnitScale](./setminorunitscale/) | Représente l'échelle de l'unité principale pour l'axe des catégories. |
| [IsVisible](./isvisible/) | Représente si l'axe est visible. |
| [SetIsVisible](./setisvisible/) | Représente si l'axe est visible. |
| [GetMajorGridLines](./getmajorgridlines/) | Représente les lignes de grille majeures sur un axe de graphique. |
| [GetMinorGridLines](./getminorgridlines/) | Représente les lignes de grille mineures sur un axe de graphique. |
| [GetHasMultiLevelLabels](./gethasmultilevellabels/) | Indique si les étiquettes doivent être affichées à plusieurs niveaux. |
| [SetHasMultiLevelLabels](./sethasmultilevellabels/) | Indique si les étiquettes doivent être affichées à plusieurs niveaux. |
| [GetAxisTexts](./getaxistexts/) | Obtient les étiquettes de l'axe après l'appel de la méthode Chart.Calculate(). |
| [GetBins](./getbins/) | Représente les intervalles sur un axe de graphique (Histogramme/Pareto) |
