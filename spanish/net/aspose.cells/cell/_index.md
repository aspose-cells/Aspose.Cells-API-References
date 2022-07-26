---
title: Cell
second_title: Referencia de API de Aspose.Cells para .NET
description: Encapsula el objeto que representa una sola celda del Libro de trabajo.
type: docs
weight: 230
url: /es/net/aspose.cells/cell/
---
## Cell class

Encapsula el objeto que representa una sola celda del Libro de trabajo.

```csharp
public class Cell
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue) { get; } | Obtiene el valor booleano contenido en la celda. |
| [Column](../../aspose.cells/cell/column) { get; } | Obtiene el número de columna (basado en cero) de la celda. |
| [Comment](../../aspose.cells/cell/comment) { get; } | Obtiene el comentario de esta celda. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink) { get; } | Indica si esta celda contiene un enlace externo. Solo se aplica cuando la celda es una celda de fórmula. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue) { get; } | Obtiene el valor DateTime contenido en la celda. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue) { get; } | Obtiene el valor de cadena con formato de esta celda según el estilo de visualización de la celda. |
| [DoubleValue](../../aspose.cells/cell/doublevalue) { get; } | Obtiene el valor doble contenido en la celda. |
| [FloatValue](../../aspose.cells/cell/floatvalue) { get; } | Obtiene el valor flotante contenido en la celda. |
| [Formula](../../aspose.cells/cell/formula) { get; set; } | Obtiene o establece una fórmula del[`Cell`](../cell) . |
| [FormulaLocal](../../aspose.cells/cell/formulalocal) { get; set; } | Obtenga la fórmula con formato local de la celda. |
| [HtmlString](../../aspose.cells/cell/htmlstring) { get; set; } | Obtiene y establece la cadena html que contiene datos y algunos formatos en esta celda. |
| [IntValue](../../aspose.cells/cell/intvalue) { get; } | Obtiene el valor entero contenido en la celda. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula) { get; } | Indica si la fórmula de la celda es una fórmula matricial. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader) { get; } | Indica que la fórmula de la celda es una fórmula de matriz y es la primera celda de la matriz. |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue) { get; } | Comprueba si el valor de esta celda es un error. |
| [IsFormula](../../aspose.cells/cell/isformula) { get; } | Representa si la celda especificada contiene fórmula. |
| [IsMerged](../../aspose.cells/cell/ismerged) { get; } | Comprueba si una celda es parte de un rango fusionado o no. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue) { get; } | Indica si el valor interno de esta celda es numérico (int, double y datetime) |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula) { get; } | Indica si la fórmula de la celda es parte de una fórmula compartida. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset) { get; } | Indica si el estilo de la celda está configurado. Si devuelve falso, significa que esta celda tiene un formato de celda predeterminado. |
| [IsTableFormula](../../aspose.cells/cell/istableformula) { get; } | Indica si esta celda es parte de la fórmula de la tabla. |
| [Name](../../aspose.cells/cell/name) { get; } | Obtiene el nombre de la celda. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype) { get; } | Representa el tipo de categoría del formato de número de esta celda. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula) { get; set; } | Obtiene o establece una fórmula R1C1 del[`Cell`](../cell) . |
| [Row](../../aspose.cells/cell/row) { get; } | Obtiene el número de fila (basado en cero) de la celda. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex) { get; } | Obtiene el índice de estilo compartido de la celda en el grupo de estilos. |
| [StringValue](../../aspose.cells/cell/stringvalue) { get; } | Obtiene el valor de cadena contenido en la celda. Si el tipo de esta celda es una cadena, devuelva el valor de la cadena en sí mismo. Para otros tipos de celda, se devolverá el valor de la cadena con formato (formateado con el estilo especificado de esta celda). El valor de la celda con formato es el mismo que puede obtener de Excel al copiar una celda como texto (como copiar la celda al editor de texto o exportar a csv). |
| [Type](../../aspose.cells/cell/type) { get; } | Representa el tipo de valor de celda. |
| [Value](../../aspose.cells/cell/value) { get; set; } | Obtiene el valor contenido en esta celda. |
| [Worksheet](../../aspose.cells/cell/worksheet) { get; } | Obtiene la hoja de cálculo principal. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate#calculate)(CalculationOptions) | Calcula la fórmula de la celda. |
| [Characters](../../aspose.cells/cell/characters)(int, int) | Devuelve un objeto Characters que representa un rango de caracteres dentro del texto de la celda. |
| [Copy](../../aspose.cells/cell/copy)(Cell) | Copia datos de una celda de origen. |
| [Equals](../../aspose.cells/cell/equals#equals)(Cell) | Comprueba si este objeto se refiere a la misma celda con otro objeto de celda. |
| override [Equals](../../aspose.cells/cell/equals#equals_1)(object) | Comprueba si este objeto hace referencia a la misma celda con otro. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange)() | Obtiene el rango de la matriz si la fórmula de la celda es una fórmula de matriz. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters)() | Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto de la celda. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters_1)(bool) | Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto de la celda. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult)() | Obtiene el resultado del formato condicional. |
| [GetDependents](../../aspose.cells/cell/getdependents)(bool) | Obtiene todas las celdas cuya fórmula hace referencia directamente a esta celda. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation)(bool) | Obtiene todas las celdas cuyo resultado calculado depende de esta celda. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle)() | Obtiene el estilo de visualización de la celda. Si esta celda también se ve afectada por otras configuraciones, como formato condicional, lista de objetos, etc., entonces el estilo de visualización puede ser diferente de cell.GetStyle(). |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle_1)(bool) | Obtiene el estilo de visualización de la celda. Si la celda tiene formato condicional, el estilo de visualización no es el mismo que el de la celda.GetStyle(). |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions)() | Obtiene las condiciones de formato que se aplican a esta celda. |
| [GetFormula](../../aspose.cells/cell/getformula)(bool, bool) | Obtenga la fórmula de esta celda. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode)() | Sirve como una función hash para un tipo particular. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue)() | Obtiene la altura del valor en unidades de píxeles. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring)(bool) | Obtiene la cadena html que contiene datos y algunos formatos en esta celda. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange)() | Devuelve un[`Range`](../range) objeto que representa un rango fusionado. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents)() | Obtiene todas las referencias que aparecen en la fórmula de esta celda. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation)() | Obtiene todos los precedentes (referencia a celdas en el libro de trabajo actual) usados por la fórmula de esta celda al calcularla. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue)(CellValueFormatStrategy) | Obtiene el valor de cadena por estrategia formateada específica. |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle)() | Obtiene el estilo de celda. |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle_1)(bool) | Si checkBorders es verdadero, verifica si los bordes de otras celdas afectarán el estilo de esta celda. |
| [GetTable](../../aspose.cells/cell/gettable)() | Obtiene la tabla que contiene esta celda. |
| [GetValidation](../../aspose.cells/cell/getvalidation)() | Obtiene la validación aplicada a esta celda. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue)() | Obtiene el valor de validación que aplicó a esta celda. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue)() | Obtiene el ancho del valor en unidades de píxeles. |
| [IsRichText](../../aspose.cells/cell/isrichtext)() | Indica si el valor de la cadena de celdas es un texto enriquecido. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue)(bool) | Pone un valor booleano en la celda. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_3)(DateTime) | Pone un valor DateTime en la celda. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_1)(double) | Pone un valor doble en la celda. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_2)(int) | Pone un valor entero en la celda. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_4)(object) | Pone un valor de objeto en la celda. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_5)(string) | Pone un valor de cadena en la celda. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_6)(string, bool) | Pone un valor de cadena en la celda y convierte el valor a otro tipo de datos si corresponde. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_7)(string, bool, bool) | Pone un valor en la celda, si corresponde, el valor se convertirá a otro tipo de datos y se restablecerá el formato de número de la celda. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula)(bool) | Eliminar fórmula matricial. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula)(string, int, int) | Establece una fórmula de matriz (fórmula de matriz heredada ingresada mediante CTRL+MAYÚS+ENTRAR en MS Excel) en un rango de celdas. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_1)(string, int, int, FormulaParseOptions) | Establece una fórmula de matriz en un rango de celdas. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | Establece una fórmula de matriz en un rango de celdas. |
| [SetCharacters](../../aspose.cells/cell/setcharacters)(FontSetting[]) | Establece el formato de texto enriquecido de la celda. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula)(string, FormulaParseOptions, bool) | Establece la fórmula de matriz dinámica y hace que la fórmula se extienda a las celdas vecinas si es posible. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | Establece la fórmula de matriz dinámica y hace que la fórmula se extienda a las celdas vecinas si es posible. |
| [SetFormula](../../aspose.cells/cell/setformula#setformula_2)(string, object) | Establecer la fórmula y el valor de la fórmula. |
| [SetFormula](../../aspose.cells/cell/setformula#setformula)(string, FormulaParseOptions, object) | Establecer la fórmula y el valor de la fórmula. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula)(string, int, int) | Establece una fórmula en un rango de celdas. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_1)(string, int, int, FormulaParseOptions) | Establece una fórmula en un rango de celdas. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | Establece una fórmula en un rango de celdas. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle)(Style) | Establece el estilo de celda. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_2)(Style, bool) | Aplicar el estilo de celda. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_1)(Style, StyleFlag) | Aplicar el estilo de celda. |
| override [ToString](../../aspose.cells/cell/tostring)() | Devuelve una cadena que representa el objeto Cell actual. |

### Ejemplos

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

// Poner una cadena en una celda
Cell cell = cells[0, 0];
cell.PutValue("Hello");

string first = cell.StringValue;
	
// Poner un entero en una celda
cell = cells["B1"];
cell.PutValue(12);

int second = cell.IntValue;

//Pon un doble en una celda
cell = cells[0, 2];
cell.PutValue(-1.234);

double third = cell.DoubleValue;

// Poner una fórmula en una celda
cell = cells["D1"];
cell.Formula = "=B1 + C1";

//Pon una fórmula combinada: "sum(average(b1,c1), b1)" a la celda en b2
cell = cells["b2"];
cell.Formula = "=sum(average(b1,c1), b1)";

//Establece el estilo de una celda
Style style = cell.GetStyle();
//Establecer color de fondo
style.BackgroundColor = Color.Yellow;
//Establecer el formato de una celda
style.Font.Name = "Courier New";
style.VerticalAlignment = TextAlignmentType.Top;
cell.SetStyle(style);



[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = exce.Worksheets(0).Cells

'Poner una cadena en una celda
Dim cell as Cell = cells(0, 0)
cell.PutValue("Hello")

Dim first as String = cell.StringValue
	
// Poner un entero en una celda
cell = cells("B1")
cell.PutValue(12)

Dim second as Integer = cell.IntValue

//Pon un doble en una celda
cell = cells(0, 2)
cell.PutValue(-1.234)

Dim third as Double = cell.DoubleValue

// Poner una fórmula en una celda
cell = cells("D1")
cell.Formula = "=B1 + C1"

//Pon una fórmula combinada: "sum(average(b1,c1), b1)" a la celda en b2
cell = cells("b2")
cell.Formula = "=sum(average(b1,c1), b1)"
	
//Establece el estilo de una celda
Dim style as Style = cell.GetStyle()

//Establecer color de fondo
style.BackgroundColor = Color.Yellow
//Establecer fuente de una celda
style.Font.Name = "Courier New"
style.VerticalAlignment = TextAlignmentType.Top
cell.SetStyle(style)
```

### Ver también

* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
