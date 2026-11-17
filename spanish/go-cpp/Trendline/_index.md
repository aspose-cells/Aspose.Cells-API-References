---
title: "Clase Trendline"
linktitle: "Trendline"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase Trendline. Encapsula el objeto que representa trendline en Go."
type: docs
weight: 200
url: /es/go-cpp/trendline/
---

## Trendline class

Represents a trendline in a chart.

```go

type Trendline struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewTrendline](./newtrendline/) | Constructs from a parent object. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [IsNameAuto](./isnameauto/) | Devuelve si Microsoft Excel determina automáticamente el nombre de la línea de tendencia. |
| [SetIsNameAuto](./setisnameauto/) | Devuelve si Microsoft Excel determina automáticamente el nombre de la línea de tendencia. |
| [GetType](./gettype/) | Devuelve el tipo de línea de tendencia. |
| [GetName](./getname/) | Devuelve el nombre de la línea de tendencia. |
| [SetName](./setname/) | Devuelve el nombre de la línea de tendencia. |
| [GetOrder](./getorder/) | Obtiene o establece el orden de la línea de tendencia (un entero mayor que 1) cuando el tipo de línea de tendencia es Polinomial. El orden debe estar entre 2 y 6. |
| [SetOrder](./setorder/) | Obtiene o establece el orden de la línea de tendencia (un entero mayor que 1) cuando el tipo de línea de tendencia es Polinomial. El orden debe estar entre 2 y 6. |
| [GetPeriod](./getperiod/) | Obtiene o establece el período para la línea de tendencia de media móvil. |
| [SetPeriod](./setperiod/) | Obtiene o establece el período para la línea de tendencia de media móvil. |
| [GetForward](./getforward/) | Obtiene o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia adelante. El número de períodos debe ser mayor o igual a cero. |
| [SetForward](./setforward/) | Obtiene o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia adelante. El número de períodos debe ser mayor o igual a cero. |
| [GetBackward](./getbackward/) | Obtiene o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia atrás. El número de períodos debe ser mayor o igual a cero. Si el tipo de gráfico es columna, el número de períodos debe estar entre 0 y 0.5. |
| [SetBackward](./setbackward/) | Obtiene o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia atrás. El número de períodos debe ser mayor o igual a cero. Si el tipo de gráfico es columna, el número de períodos debe estar entre 0 y 0.5. |
| [GetDisplayEquation](./getdisplayequation/) | Representa si la ecuación de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que el valor R al cuadrado). Establecer esta propiedad en True activa automáticamente las etiquetas de datos. |
| [SetDisplayEquation](./setdisplayequation/) | Representa si la ecuación de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que el valor R al cuadrado). Establecer esta propiedad en True activa automáticamente las etiquetas de datos. |
| [GetDisplayRSquared](./getdisplayrsquared/) | Representa si el valor R al cuadrado de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que la ecuación). Establecer esta propiedad en True activa automáticamente las etiquetas de datos. |
| [SetDisplayRSquared](./setdisplayrsquared/) | Representa si el valor R al cuadrado de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que la ecuación). Establecer esta propiedad en True activa automáticamente las etiquetas de datos. |
| [GetIntercept](./getintercept/) | Obtiene o establece el punto donde la línea de tendencia cruza el eje de valores. |
| [SetIntercept](./setintercept/) | Obtiene o establece el punto donde la línea de tendencia cruza el eje de valores. |
| [GetDataLabels](./getdatalabels/) | Representa el objeto DataLabels para la serie especificada. |
| [GetLegendEntry](./getlegendentry/) | Obtiene la entrada de leyenda según esta línea de tendencia. |
| [GetCompoundType](./getcompoundtype/) | Specifies the compound line type |
| [SetCompoundType](./setcompoundtype/) | Specifies the compound line type |
| [GetDashType](./getdashtype/) | Specifies the dash line type |
| [SetDashType](./setdashtype/) | Specifies the dash line type |
| [GetCapType](./getcaptype/) | Specifies the ending caps. |
| [SetCapType](./setcaptype/) | Specifies the ending caps. |
| [GetJoinType](./getjointype/) | Specifies the joining caps. |
| [SetJoinType](./setjointype/) | Specifies the joining caps. |
| [GetBeginType](./getbegintype/) | Specifies an arrowhead for the begin of a line. |
| [SetBeginType](./setbegintype/) | Specifies an arrowhead for the begin of a line. |
| [GetEndType](./getendtype/) | Specifies an arrowhead for the end of a line. |
| [SetEndType](./setendtype/) | Specifies an arrowhead for the end of a line. |
| [GetBeginArrowLength](./getbeginarrowlength/) | Specifies the length of the arrowhead for the begin of a line. |
| [SetBeginArrowLength](./setbeginarrowlength/) | Specifies the length of the arrowhead for the begin of a line. |
| [GetEndArrowLength](./getendarrowlength/) | Specifies the length of the arrowhead for the end of a line. |
| [SetEndArrowLength](./setendarrowlength/) | Specifies the length of the arrowhead for the end of a line. |
| [GetBeginArrowWidth](./getbeginarrowwidth/) | Specifies the width of the arrowhead for the begin of a line. |
| [SetBeginArrowWidth](./setbeginarrowwidth/) | Specifies the width of the arrowhead for the begin of a line. |
| [GetEndArrowWidth](./getendarrowwidth/) | Specifies the width of the arrowhead for the end of a line. |
| [SetEndArrowWidth](./setendarrowwidth/) | Specifies the width of the arrowhead for the end of a line. |
| [GetThemeColor](./getthemecolor/) | Gets and sets the theme color. |
| [SetThemeColor](./setthemecolor/) | Gets and sets the theme color. |
| [GetColor](./getcolor/) | Represents the Color of the line. |
| [SetColor](./setcolor/) | Represents the Color of the line. |
| [GetTransparency](./gettransparency/) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [SetTransparency](./settransparency/) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [GetStyle](./getstyle/) | Represents the style of the line. |
| [SetStyle](./setstyle/) | Represents the style of the line. |
| [GetWeight](./getweight/) | Gets or sets the WeightType of the line. |
| [SetWeight](./setweight/) | Gets or sets the WeightType of the line. |
| [GetWeightPt](./getweightpt/) | Gets or sets the weight of the line in unit of points. |
| [SetWeightPt](./setweightpt/) | Gets or sets the weight of the line in unit of points. |
| [GetWeightPx](./getweightpx/) | Gets or sets the weight of the line in unit of pixels. |
| [SetWeightPx](./setweightpx/) | Gets or sets the weight of the line in unit of pixels. |
| [GetFormattingType](./getformattingtype/) | Gets or sets format type. |
| [SetFormattingType](./setformattingtype/) | Gets or sets format type. |
| [IsAutomaticColor](./isautomaticcolor/) | Indicates whether the color of line is automatic assigned. |
| [IsVisible](./isvisible/) | Represents whether the line is visible. |
| [SetIsVisible](./setisvisible/) | Represents whether the line is visible. |
| [IsAuto](./isauto/) | Indicates whether this line style is auto assigned. |
| [SetIsAuto](./setisauto/) | Indicates whether this line style is auto assigned. |
| [GetGradientFill](./getgradientfill/) | Represents gradient fill. |
