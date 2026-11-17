---
title: "Clase Axis"
linktitle: "Axis"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase Axis. Encapsula el objeto que representa el eje en Go."
type: docs
weight: 200
url: /es/go-cpp/axis/
---

## Axis class

Encapsulates the object that represents an axis of a chart.

```go

type Axis struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetArea](./getarea/) | Obtiene el área. |
| [IsAutomaticMinValue](./isautomaticminvalue/) | Indica si el valor mínimo se asigna automáticamente. |
| [SetIsAutomaticMinValue](./setisautomaticminvalue/) | Indica si el valor mínimo se asigna automáticamente. |
| [GetMinValue](./getminvalue/) | Representa el valor mínimo en el eje de valores. |
| [SetMinValue](./setminvalue/) | Representa el valor mínimo en el eje de valores. |
| [IsAutomaticMaxValue](./isautomaticmaxvalue/) | Indica si el valor máximo se asigna automáticamente. |
| [SetIsAutomaticMaxValue](./setisautomaticmaxvalue/) | Indica si el valor máximo se asigna automáticamente. |
| [GetMaxValue](./getmaxvalue/) | Representa el valor máximo en el eje de valores. |
| [SetMaxValue](./setmaxvalue/) | Representa el valor máximo en el eje de valores. |
| [IsAutomaticMajorUnit](./isautomaticmajorunit/) | Indica si la unidad mayor del eje se asigna automáticamente. |
| [SetIsAutomaticMajorUnit](./setisautomaticmajorunit/) | Indica si la unidad mayor del eje se asigna automáticamente. |
| [GetMajorUnit](./getmajorunit/) | Representa las unidades mayores del eje. |
| [SetMajorUnit](./setmajorunit/) | Representa las unidades mayores del eje. |
| [IsAutomaticMinorUnit](./isautomaticminorunit/) | Indica si la unidad menor del eje se asigna automáticamente. |
| [SetIsAutomaticMinorUnit](./setisautomaticminorunit/) | Indica si la unidad menor del eje se asigna automáticamente. |
| [GetMinorUnit](./getminorunit/) | Representa las unidades menores del eje. |
| [SetMinorUnit](./setminorunit/) | Representa las unidades menores del eje. |
| [GetAxisLine](./getaxisline/) | Obtiene la apariencia de un Axis. |
| [GetMajorTickMark](./getmajortickmark/) | Representa el tipo de marca de graduación mayor para el eje especificado. |
| [SetMajorTickMark](./setmajortickmark/) | Representa el tipo de marca de graduación mayor para el eje especificado. |
| [GetMinorTickMark](./getminortickmark/) | Representa el tipo de marca de graduación menor para el eje especificado. |
| [SetMinorTickMark](./setminortickmark/) | Representa el tipo de marca de graduación menor para el eje especificado. |
| [GetTickLabelPosition](./getticklabelposition/) | Representa la posición de las etiquetas de marcas de graduación en el eje especificado. |
| [SetTickLabelPosition](./setticklabelposition/) | Representa la posición de las etiquetas de marcas de graduación en el eje especificado. |
| [GetCrossAt](./getcrossat/) | Representa el punto en el eje de valores donde el eje de categorías lo cruza. |
| [SetCrossAt](./setcrossat/) | Representa el punto en el eje de valores donde el eje de categorías lo cruza. |
| [GetCrossType](./getcrosstype/) | Representa el CrossType en el eje especificado donde cruza el otro eje. |
| [SetCrossType](./setcrosstype/) | Representa el CrossType en el eje especificado donde cruza el otro eje. |
| [GetLogBase](./getlogbase/) | Representa la base logarítmica. El valor predeterminado es 10. |
| [SetLogBase](./setlogbase/) | Representa la base logarítmica. El valor predeterminado es 10. |
| [IsLogarithmic](./islogarithmic/) | Representa si el tipo de escala del eje de valores es logarítmico o no. |
| [SetIsLogarithmic](./setislogarithmic/) | Representa si el tipo de escala del eje de valores es logarítmico o no. |
| [IsPlotOrderReversed](./isplotorderreversed/) | Representa si Microsoft Excel traza los puntos de datos de último a primero. |
| [SetIsPlotOrderReversed](./setisplotorderreversed/) | Representa si Microsoft Excel traza los puntos de datos de último a primero. |
| [GetAxisBetweenCategories](./getaxisbetweencategories/) | Representa si el eje de valores cruza el eje de categorías entre categorías. |
| [SetAxisBetweenCategories](./setaxisbetweencategories/) | Representa si el eje de valores cruza el eje de categorías entre categorías. |
| [GetTickLabels](./getticklabels/) | Devuelve un objeto TickLabels que representa las etiquetas de marcas de graduación para el eje especificado. |
| [GetTickLabelSpacing](./getticklabelspacing/) | Representa el número de categorías o series entre las etiquetas de marcas de graduación. Se aplica solo a ejes de categoría y series. |
| [SetTickLabelSpacing](./setticklabelspacing/) | Representa el número de categorías o series entre las etiquetas de marcas de graduación. Se aplica solo a ejes de categoría y series. |
| [IsAutoTickLabelSpacing](./isautoticklabelspacing/) | Indica si el espaciado de la etiqueta de marca es automático |
| [SetIsAutoTickLabelSpacing](./setisautoticklabelspacing/) | Indica si el espaciado de la etiqueta de marca es automático |
| [GetTickMarkSpacing](./gettickmarkspacing/) | Devuelve o establece el número de categorías o series entre marcas de graduación. Se aplica solo a ejes de categoría y series. |
| [SetTickMarkSpacing](./settickmarkspacing/) | Devuelve o establece el número de categorías o series entre marcas de graduación. Se aplica solo a ejes de categoría y series. |
| [GetDisplayUnit](./getdisplayunit/) | Representa la etiqueta de unidad para el eje especificado. |
| [SetDisplayUnit](./setdisplayunit/) | Representa la etiqueta de unidad para el eje especificado. |
| [GetCustomDisplayUnit](./getcustomdisplayunit/) | Especifica un valor personalizado para la unidad de visualización. |
| [SetCustomDisplayUnit](./setcustomdisplayunit/) | Especifica un valor personalizado para la unidad de visualización. |
| [GetDisplayUnitLabel](./getdisplayunitlabel/) | Representa una etiqueta de unidad en un eje del gráfico especificado. Las etiquetas de unidad son útiles para graficar valores grandes, por ejemplo, en millones o miles de millones. |
| [IsDisplayUnitLabelShown](./isdisplayunitlabelshown/) | Representa si la etiqueta de unidad de visualización se muestra en el eje especificado. |
| [SetIsDisplayUnitLabelShown](./setisdisplayunitlabelshown/) | Representa si la etiqueta de unidad de visualización se muestra en el eje especificado. |
| [GetTitle](./gettitle/) | Obtiene el título de este eje en el gráfico. |
| [GetCategoryType](./getcategorytype/) | Representa el tipo del eje de categoría. |
| [SetCategoryType](./setcategorytype/) | Representa el tipo del eje de categoría. |
| [GetBaseUnitScale](./getbaseunitscale/) | Representa la escala de unidad base para el eje de categoría. |
| [SetBaseUnitScale](./setbaseunitscale/) | Representa la escala de unidad base para el eje de categoría. |
| [GetMajorUnitScale](./getmajorunitscale/) | Representa la escala de unidad mayor para el eje de categoría. |
| [SetMajorUnitScale](./setmajorunitscale/) | Representa la escala de unidad mayor para el eje de categoría. |
| [GetMinorUnitScale](./getminorunitscale/) | Representa la escala de unidad mayor para el eje de categoría. |
| [SetMinorUnitScale](./setminorunitscale/) | Representa la escala de unidad mayor para el eje de categoría. |
| [IsVisible](./isvisible/) | Representa si el eje es visible. |
| [SetIsVisible](./setisvisible/) | Representa si el eje es visible. |
| [GetMajorGridLines](./getmajorgridlines/) | Representa las líneas de cuadrícula mayores en el eje de un gráfico. |
| [GetMinorGridLines](./getminorgridlines/) | Representa las líneas de cuadrícula menores en el eje de un gráfico. |
| [GetHasMultiLevelLabels](./gethasmultilevellabels/) | Indica si las etiquetas se mostrarán como multinivel. |
| [SetHasMultiLevelLabels](./sethasmultilevellabels/) | Indica si las etiquetas se mostrarán como multinivel. |
| [GetAxisTexts](./getaxistexts/) | Obtiene las etiquetas del eje después de llamar al método Chart.Calculate(). |
| [GetBins](./getbins/) | Representa los contenedores en el eje de un gráfico (Histograma/Pareto) |
