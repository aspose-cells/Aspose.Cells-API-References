---
title: "Clase FormatCondition"
linktitle: "FormatCondition"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase FormatCondition. Encapsula el objeto que representa formatcondition en Go."
type: docs
weight: 200
url: /es/go-cpp/formatcondition/
---

## FormatCondition class

Represents conditional formatting condition.

```go

type FormatCondition struct  {
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
| [GetFormula1_Bool_Bool](./getformula1_bool_bool/) | Obtiene el valor o expresión asociado a esta condición de formato. |
| [GetFormula2_Bool_Bool](./getformula2_bool_bool/) | Obtiene el valor o expresión asociado a esta condición de formato. |
| [GetFormula1_Bool_Bool_Int_Int](./getformula1_bool_bool_int_int/) | Obtiene el valor o expresión del formato condicional de la celda. |
| [GetFormula2_Bool_Bool_Int_Int](./getformula2_bool_bool_int_int/) | Obtiene el valor o expresión del formato condicional de la celda. |
| [SetFormulas](./setformulas/) | Establece el valor o expresión asociado a esta condición de formato. |
| [SetFormula1_String_Bool_Bool](./setformula1_string_bool_bool/) | Establece el valor o expresión asociado a esta condición de formato. |
| [SetFormula2_String_Bool_Bool](./setformula2_string_bool_bool/) | Establece el valor o expresión asociado a esta condición de formato. |
| [GetFormula1](./getformula1/) | Obtiene y establece el valor o expresión asociado al formato condicional. |
| [SetFormula1_String](./setformula1_string/) | Obtiene y establece el valor o expresión asociado al formato condicional. |
| [GetFormula1_Int_Int](./getformula1_int_int/) | Obtiene la fórmula del formato condicional de la celda. |
| [GetFormula2](./getformula2/) | Obtiene y establece el valor o expresión asociado al formato condicional. |
| [SetFormula2_String](./setformula2_string/) | Obtiene y establece el valor o expresión asociado al formato condicional. |
| [GetFormula2_Int_Int](./getformula2_int_int/) | Obtiene la fórmula del formato condicional de la celda. |
| [GetOperator](./getoperator/) | Obtiene y establece el tipo de operador del formato condicional. |
| [SetOperator](./setoperator/) | Obtiene y establece el tipo de operador del formato condicional. |
| [GetStopIfTrue](./getstopiftrue/) | Verdadero, ninguna regla con menor prioridad puede aplicarse sobre esta regla, cuando esta regla se evalúa como verdadera. Solo se aplica a Excel 2007; |
| [SetStopIfTrue](./setstopiftrue/) | Verdadero, ninguna regla con menor prioridad puede aplicarse sobre esta regla, cuando esta regla se evalúa como verdadera. Solo se aplica a Excel 2007; |
| [GetPriority](./getpriority/) | La prioridad de esta regla de formato condicional. Este valor se usa para determinar qué formato debe evaluarse y renderizarse. Los valores numéricos más bajos tienen mayor prioridad que los valores numéricos más altos, donde '1' es la prioridad más alta. |
| [SetPriority](./setpriority/) | La prioridad de esta regla de formato condicional. Este valor se usa para determinar qué formato debe evaluarse y renderizarse. Los valores numéricos más bajos tienen mayor prioridad que los valores numéricos más altos, donde '1' es la prioridad más alta. |
| [GetStyle](./getstyle/) | Obtiene o establece el estilo de los rangos de celdas con formato condicional. |
| [SetStyle](./setstyle/) | Obtiene o establece el estilo de los rangos de celdas con formato condicional. |
| [GetType](./gettype/) | Obtiene y establece el tipo de formato condicional. |
| [SetType](./settype/) | Obtiene y establece el tipo de formato condicional. |
| [GetIconSet](./geticonset/) | Obtiene la instancia "IconSet" del formato condicional. El tipo IconSetType de la instancia predeterminada es TrafficLights31. Válido solo para type = IconSet. |
| [GetDataBar](./getdatabar/) | Obtiene la instancia "DataBar" del formato condicional. El color de la instancia predeterminada es azul. Válido solo para type = DataBar. |
| [GetColorScale](./getcolorscale/) | Obtiene la instancia "ColorScale" del formato condicional. La instancia predeterminada es una "green-yellow-red" 3ColorScale. Válido solo para type = ColorScale. |
| [GetTop10](./gettop10/) | Obtiene la instancia "Top10" del formato condicional. La regla de la instancia predeterminada resalta las celdas cuyos valores están en el rango superior del 10%. Válido solo para type = Top10. |
| [GetAboveAverage](./getaboveaverage/) | Obtiene la instancia "AboveAverage" del formato condicional. La regla de la instancia predeterminada resalta las celdas que están por encima del promedio de todos los valores en el rango. Válido solo para type = AboveAverage. |
| [GetText](./gettext/) | El valor de texto en una regla de formato condicional "text contains". Válido solo para type = containsText, notContainsText, beginsWith y endsWith. El valor predeterminado es null. |
| [SetText](./settext/) | El valor de texto en una regla de formato condicional "text contains". Válido solo para type = containsText, notContainsText, beginsWith y endsWith. El valor predeterminado es null. |
| [GetTimePeriod](./gettimeperiod/) | El período de tiempo aplicable en una regla de formato condicional "date occurrin". Válido solo para type = timePeriod. El valor predeterminado es TimePeriodType.Today. |
| [SetTimePeriod](./settimeperiod/) | El período de tiempo aplicable en una regla de formato condicional "date occurrin". Válido solo para type = timePeriod. El valor predeterminado es TimePeriodType.Today. |
