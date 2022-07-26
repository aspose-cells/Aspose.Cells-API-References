---
title: FormatCondition
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa la condición de formato condicional.
type: docs
weight: 3560
url: /es/net/aspose.cells/formatcondition/
---
## FormatCondition class

Representa la condición de formato condicional.

```csharp
public class FormatCondition
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage) { get; } | Obtenga la instancia "AboveAverage" del formato condicional. La regla de la instancia predeterminada resalta las celdas que están por encima del promedio para todos los valores en el rango. Válido solo para el tipo = AboveAverage. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale) { get; } | Obtenga la instancia "ColorScale" del formato condicional. La instancia predeterminada es una 3ColorScale "verde-amarillo-rojo". Válido solo para el tipo = ColorScale. |
| [DataBar](../../aspose.cells/formatcondition/databar) { get; } | Obtener la instancia "DataBar" del formato condicional. El color predeterminado de la instancia es azul. Válido solo para el tipo DataBar. |
| [Formula1](../../aspose.cells/formatcondition/formula1) { get; set; } | Obtiene y establece el valor o la expresión asociada con el formato condicional. |
| [Formula2](../../aspose.cells/formatcondition/formula2) { get; set; } | Obtiene y establece el valor o la expresión asociada con el formato condicional. |
| [IconSet](../../aspose.cells/formatcondition/iconset) { get; } | Obtenga la instancia "IconSet" del formato condicional. El IconSetType de la instancia predeterminada es TrafficLights31. Válido solo para el tipo = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator) { get; set; } | Obtiene y establece el tipo de operador de formato condicional. |
| [Priority](../../aspose.cells/formatcondition/priority) { get; set; } | La prioridad de esta regla de formato condicional. Este valor se utiliza para determinar qué formato se debe evaluar y representar. Los valores numéricos más bajos tienen mayor prioridad que valores numéricos más altos, donde '1' es la prioridad más alta. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue) { get; set; } | Verdadero, no se pueden aplicar reglas con menor prioridad sobre esta regla, cuando esta regla se evalúa como verdadera. Solo se aplica a Excel 2007; |
| [Style](../../aspose.cells/formatcondition/style) { get; set; } | Obtiene o establece el estilo de los rangos de celdas con formato condicional. |
| [Text](../../aspose.cells/formatcondition/text) { get; set; } | El valor de texto en una regla de formato condicional "el texto contiene". Válido solo para tipo = contiene texto, no contiene texto, comienza con y termina con. El valor predeterminado es nulo. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod) { get; set; } | El período de tiempo aplicable en una regla de formato condicional de "fecha que ocurre...". Válido solo para tipo = timePeriod. El valor predeterminado es TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10) { get; } | Obtener la instancia "Top10" del formato condicional. La regla de la instancia predeterminada resalta las celdas cuyos valores caen en el paréntesis de los 10 primeros. Válido solo para el tipo Top10. |
| [Type](../../aspose.cells/formatcondition/type) { get; set; } | Obtiene y establece si el formato condicional Type. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1)(bool, bool) | Obtiene el valor o la expresión asociada a esta condición de formato. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_2)(int, int) | Obtiene la fórmula del formato condicional de la celda. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_1)(bool, bool, int, int) | Obtiene el valor o expresión del formato condicional de la celda. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2)(bool, bool) | Obtiene el valor o la expresión asociada a esta condición de formato. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_2)(int, int) | Obtiene la fórmula del formato condicional de la celda. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_1)(bool, bool, int, int) | Obtiene el valor o expresión del formato condicional de la celda. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1)(string, bool, bool) | Establece el valor o la expresión asociada a esta condición de formato. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2)(string, bool, bool) | Establece el valor o la expresión asociada a esta condición de formato. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas)(string, string, bool, bool) | Establece el valor o la expresión asociada a esta condición de formato. |

### Ejemplos

```csharp

[C#]
// Instanciando un objeto Workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
 
//Agrega un formato condicional vacío
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
 
//Establece el rango de formato condicional.
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.AddArea(ca);
 
ca = new CellArea();
ca.StartRow = 1;
ca.EndRow = 1;
ca.StartColumn = 1;
ca.EndColumn = 1;
fcs.AddArea(ca);
 
//Agrega condición.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
 
//Agrega condición.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
 
//Establece el color de fondo.
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
 
//Guardando el archivo de Excel
workbook.Save("output.xls");

[VB.NET]

'Crear una instancia de un objeto Workbook
Dim workbook As Workbook = New Workbook()
Dim sheet As Worksheet = workbook.Worksheets(0)
 
' Agrega un formato condicional vacío
Dim index As Integer = sheet.ConditionalFormattings.Add()
Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)
 
'Establece el rango de formato condicional.
Dim ca As CellArea = New CellArea()
ca.StartRow = 0
ca.EndRow = 0
ca.StartColumn = 0
ca.EndColumn = 0
fcs.AddArea(ca)
ca = New CellArea()
ca.StartRow = 1
ca.EndRow = 1
ca.StartColumn = 1
ca.EndColumn = 1
fcs.AddArea(ca)
 
'Agrega condición.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100")
 
'Agrega condición.
Dim conditionIndex2 As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100")
 
'Establece el color de fondo.
Dim fc As FormatCondition = fcs(conditionIndex)
fc.Style.BackgroundColor = Color.Red
 
'Guardar el archivo de Excel
workbook.Save("output.xls")
```

### Ver también

* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
