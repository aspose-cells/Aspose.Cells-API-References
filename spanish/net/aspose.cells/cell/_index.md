---
title: "Clase Cell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Cell. Encapsula el objeto que representa una única celda de libro de trabajo"
type: docs
url: /es/net/aspose.cells/cell/
---
## Cell class

Encapsula el objeto que representa una única celda de Workbook.

```csharp
public class Cell
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue/) { get; } | Obtiene el valor booleano contenido en la celda. |
| [Column](../../aspose.cells/cell/column/) { get; } | Obtiene el número de columna (basado en cero) de la celda. |
| [Comment](../../aspose.cells/cell/comment/) { get; } | Obtiene el comentario de esta celda. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink/) { get; } | Indica si esta celda contiene un enlace externo. Solo se aplica cuando la celda es una celda de fórmula. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue/) { get; } | Obtiene el valor DateTime contenido en la celda. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue/) { get; } | Obtiene el valor de cadena formateada de esta celda según el estilo de visualización de la celda. |
| [DoubleValue](../../aspose.cells/cell/doublevalue/) { get; } | Obtiene el valor double contenido en la celda. |
| [EmbeddedImage](../../aspose.cells/cell/embeddedimage/) { get; set; } | Obtiene y establece la imagen incrustada en la celda. |
| [FloatValue](../../aspose.cells/cell/floatvalue/) { get; } | Obtiene el valor float contenido en la celda. |
| [Formula](../../aspose.cells/cell/formula/) { get; set; } | Obtiene o establece una fórmula de la `Cell`. |
| [FormulaLocal](../../aspose.cells/cell/formulalocal/) { get; set; } | Obtenga la fórmula formateada según la configuración regional de la celda. |
| [HasCustomFunction](../../aspose.cells/cell/hascustomfunction/) { get; } | Comprueba si hay una función personalizada (función no compatible) en la fórmula de esta celda. |
| [HasCustomStyle](../../aspose.cells/cell/hascustomstyle/) { get; } | Indica si esta celda tiene configuraciones de estilo personalizadas (diferentes de la predeterminada heredada de la fila, columna o libro de trabajo correspondiente). |
| [HtmlString](../../aspose.cells/cell/htmlstring/) { get; set; } | Obtiene y establece la cadena html que contiene datos y algunos formatos en esta celda. |
| [IntValue](../../aspose.cells/cell/intvalue/) { get; } | Obtiene el valor entero contenido en la celda. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula/) { get; } | Indica si la fórmula de la celda es una fórmula de matriz. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader/) { get; } | Indica que la fórmula de la celda es una fórmula de matriz y que es la primera celda de la matriz. |
| [IsCheckBoxStyle](../../aspose.cells/cell/ischeckboxstyle/) { get; set; } | Indica si se establece esta celda como una casilla de verificación. |
| [IsDynamicArrayFormula](../../aspose.cells/cell/isdynamicarrayformula/) { get; } | Indica si la fórmula de la celda es una fórmula de matriz dinámica (true) o una fórmula de matriz heredada (false). |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue/) { get; } | Comprueba si el valor de esta celda es un error. |
| [IsFormula](../../aspose.cells/cell/isformula/) { get; } | Representa si la celda especificada contiene una fórmula. |
| [IsInArray](../../aspose.cells/cell/isinarray/) { get; } | (**Obsolete.**) Indica si la fórmula de la celda es una fórmula de matriz. |
| [IsInTable](../../aspose.cells/cell/isintable/) { get; } | (**Obsolete.**) Indica si esta celda forma parte de una fórmula de tabla. |
| [IsMerged](../../aspose.cells/cell/ismerged/) { get; } | Comprueba si una celda forma parte de un rango combinado o no. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue/) { get; } | Indica si el valor de esta celda es numérico (int, double y datetime) |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula/) { get; } | Indica si la fórmula de la celda forma parte de una fórmula compartida. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset/) { get; } | Indica si el estilo de la celda está establecido. Si devuelve false, significa que esta celda tiene un formato de celda predeterminado. |
| [IsTableFormula](../../aspose.cells/cell/istableformula/) { get; } | Indica si esta celda forma parte de una fórmula de tabla. |
| [Name](../../aspose.cells/cell/name/) { get; } | Obtiene el nombre de la celda. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype/) { get; } | Representa el tipo de categoría del formato numérico de esta celda. |
| [Picture](../../aspose.cells/cell/picture/) { get; } | Obtiene una instancia de [`Picture`](../../aspose.cells.drawing/picture/) para representar la imagen incrustada en esta celda o null si no hay ninguna imagen incrustada para esta celda. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula/) { get; set; } | Obtiene o establece una fórmula R1C1 de la `Cell`. |
| [Row](../../aspose.cells/cell/row/) { get; } | Obtiene el número de fila (basado en cero) de la celda. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex/) { get; } | Obtiene el índice de estilo compartido de la celda en el pool de estilos. |
| [StringValue](../../aspose.cells/cell/stringvalue/) { get; } | Obtiene el valor de cadena contenido en la celda. Si el tipo de esta celda es cadena, entonces devuelve el propio valor de cadena. Para otros tipos de celda, se devolverá el valor de cadena formateado (formateado con el estilo especificado de esta celda). El valor de celda formateado es el mismo que se puede obtener de Excel al copiar una celda como texto (como copiar la celda a un editor de texto o exportar a csv). |
| [StringValueWithoutFormat](../../aspose.cells/cell/stringvaluewithoutformat/) { get; } | (**Obsolete.**) Obtiene el valor de la celda como cadena sin ningún formato. |
| [Type](../../aspose.cells/cell/type/) { get; } | Representa el tipo de valor de la celda. |
| [Value](../../aspose.cells/cell/value/) { get; set; } | Obtiene/establece el valor contenido en esta celda. |
| [Worksheet](../../aspose.cells/cell/worksheet/) { get; } | Obtiene la hoja de cálculo principal. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate/)(CalculationOptions) | Calcula la fórmula de la celda. |
| [Characters](../../aspose.cells/cell/characters/)(int, int) | Devuelve un objeto Characters que representa un rango de caracteres dentro del texto de la celda. |
| [Copy](../../aspose.cells/cell/copy/)(Cell) | Copia datos de una celda origen. |
| [Equals](../../aspose.cells/cell/equals/#equals)(Cell) | Comprueba si este objeto se refiere a la misma celda que otro objeto de celda. |
| override [Equals](../../aspose.cells/cell/equals/#equals_1)(object) | Comprueba si este objeto se refiere a la misma celda que otro. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange/)() | Obtiene el rango de matriz si la fórmula de la celda es una fórmula de matriz. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters)() | Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto de la celda. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters_1)(bool) | Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto de la celda. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult/)() | Obtén el resultado del formato condicional. |
| [GetDependents](../../aspose.cells/cell/getdependents/)(bool) | Obtén todas las celdas cuya fórmula hace referencia directa a esta celda. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation/)(bool) | Obtiene todas las celdas cuyo resultado calculado depende de esta celda. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle)() | Obtiene el estilo de visualización de esta celda. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_2)(bool) | Obtiene el estilo de visualización de esta celda. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_1)(BorderType) | Obtiene el estilo de visualización de esta celda. |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions/)() | Obtiene las condiciones de formato que se aplican a esta celda. |
| [GetFormula](../../aspose.cells/cell/getformula/)(bool, bool) | Obtén la fórmula de esta celda. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode/)() | Sirve como función hash para un tipo particular. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue/)() | Obtiene la altura del valor en unidades de píxeles. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring/)(bool) | Obtiene la cadena HTML que contiene datos y algunos formatos en esta celda. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs)() | (**Obsolete.**) Obtén todas las celdas que hacen referencia directa a esta celda y que necesitan ser actualizadas cuando esta celda se modifica. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs_1)(bool) | (**Obsolete.**) Obtén todas las celdas que serán actualizadas cuando esta celda se modifique. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange/)() | Devuelve un objeto [`Range`](../range/) que representa un rango combinado. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents/)() | Obtiene todas las referencias que aparecen en la fórmula de esta celda. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation/)() | Obtiene todos los precedentes (referencia a celdas en el libro actual) utilizados por la fórmula de esta celda al calcularla. |
| [GetRichValue](../../aspose.cells/cell/getrichvalue/)() | Obtiene el valor enriquecido de la celda. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue/)(CellValueFormatStrategy) | Obtiene el valor de cadena mediante una estrategia de formato específica. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle)() | Obtiene el estilo de la celda. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle_1)(bool) | Si checkBorders es verdadero, verifica si los bordes de otras celdas afectarán el estilo de esta celda. |
| [GetTable](../../aspose.cells/cell/gettable/)() | Obtiene la tabla que contiene esta celda. |
| [GetValidation](../../aspose.cells/cell/getvalidation/)() | Obtiene la validación aplicada a esta celda. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue/)() | Obtiene el valor de validación que se aplica a esta celda. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue/)() | Obtiene el ancho del valor en unidades de píxeles. |
| [InsertText](../../aspose.cells/cell/inserttext/)(int, string) | Inserta algunos caracteres en la celda. Si la celda tiene formato enriquecido, este método puede conservar el formato original. |
| [IsRichText](../../aspose.cells/cell/isrichtext/)() | Indica si el valor de cadena de esta celda es un texto con formato enriquecido. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue)(bool) | Coloca un valor booleano en la celda. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_3)(DateTime) | Coloca un valor DateTime en la celda. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_1)(double) | Coloca un valor double en la celda. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_2)(int) | Coloca un valor entero en la celda. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_4)(object) | Coloca un valor objeto en la celda. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_5)(string) | Coloca un valor de cadena en la celda. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_6)(string, bool) | Coloca un valor de cadena en la celda y convierte el valor a otro tipo de datos si es apropiado. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_7)(string, bool, bool) | Coloca un valor en la celda; si es apropiado, el valor se convertirá a otro tipo de datos y el formato numérico de la celda se restablecerá. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula/)(bool) | Elimina la fórmula de matriz. |
| [Replace](../../aspose.cells/cell/replace/)(string, string, ReplaceOptions) | Reemplaza el texto de la celda con opciones. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula)(string, int, int) | Establece una fórmula de matriz (fórmula de matriz heredada ingresada mediante CTRL+SHIFT+ENTER en MS Excel) a un rango de celdas. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_1)(string, int, int, FormulaParseOptions) | Establece una fórmula de matriz a un rango de celdas. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_3)(string, int, int, bool, bool) | (**Obsoleto.**) Establece una fórmula de matriz a un rango de celdas. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | Establece una fórmula de matriz a un rango de celdas. |
| [SetCharacters](../../aspose.cells/cell/setcharacters/)(FontSetting[]) | Establece el formato de texto enriquecido de la celda. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula)(string, FormulaParseOptions, bool) | Establece una fórmula de matriz dinámica y hace que la fórmula se desborde a celdas vecinas si es posible. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | Establece una fórmula de matriz dinámica y hace que la fórmula se desborde a celdas vecinas si es posible. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_2)(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) | Establece una fórmula de matriz dinámica y hace que la fórmula se desborde a celdas vecinas si es posible. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula)(string, FormulaParseOptions) | Establece la fórmula y el valor (resultado calculado) de la fórmula. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_3)(string, object) | Establece la fórmula y el valor (resultado calculado) de la fórmula. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_1)(string, FormulaParseOptions, object) | Establece la fórmula y el valor (resultado calculado) de la fórmula. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_2)(string, bool, bool, object) | (**Obsoleto.**) Establece la fórmula y el valor de la fórmula. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula)(string, int, int) | Establece fórmulas compartidas a un rango de celdas. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_1)(string, int, int, FormulaParseOptions) | Establece fórmulas compartidas a un rango de celdas. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_3)(string, int, int, bool, bool) | (**Obsoleto.**) Establece una fórmula a un rango de celdas. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | Establece fórmulas compartidas a un rango de celdas. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle)(Style) | Establece el estilo de la celda. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_2)(Style, bool) | Aplica la propiedad modificada del estilo a la celda. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_1)(Style, StyleFlag) | Aplicar el estilo de celda basado en banderas. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_2)(int, int, string, bool, object[][]) | Crear tabla de datos de una variable para el rango dado comenzando desde esta celda. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_3)(int, int, string, string, object[][]) | Crear tabla de datos de dos variables para el rango dado comenzando desde esta celda. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula)(int, int, int, int, bool, object[][]) | Crear tabla de datos de una variable para el rango dado comenzando desde esta celda. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_1)(int, int, int, int, int, int, object[][]) | Crear tabla de datos de dos variables para el rango dado comenzando desde esta celda. |
| [ToJson](../../aspose.cells/cell/tojson/)() | Convertir `Cell` a datos estructurados JSON. |
| override [ToString](../../aspose.cells/cell/tostring/)() | Devuelve una cadena que representa el objeto Cell actual. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellDemo
    {
        public static void CellExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            // Acceder a la colección de celdas
            Cells cells = worksheet.Cells;

            // Insertar una cadena en una celda
            Cell cell = cells[0, 0];
            cell.PutValue("Hello");

            // Insertar un entero en una celda
            cell = cells["B1"];
            cell.PutValue(12);

            // Insertar un doble en una celda
            cell = cells[0, 2];
            cell.PutValue(-1.234);

            // Insertar una fórmula en una celda
            cell = cells["D1"];
            cell.Formula = "=B1 + C1";

            // Insertar una fórmula combinada: "sum(average(b1,c1), b1)" en la celda b2
            cell = cells["B2"];
            cell.Formula = "=sum(average(b1,c1), b1)";

            // Establecer el estilo de una celda
            Style style = cell.GetStyle();
            // Establecer el color de fondo
            style.BackgroundColor = System.Drawing.Color.Yellow;
            // Establecer la fuente de una celda
            style.Font.Name = "Courier New";
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("CellExample.xlsx");
            workbook.Save("CellExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


