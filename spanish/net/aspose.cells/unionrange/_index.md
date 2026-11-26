---
title: "Clase UnionRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.UnionRange. Representa un rango de unión"
type: docs
url: /es/net/aspose.cells/unionrange/
---
## UnionRange class

Representa un rango de unión.

```csharp
public class UnionRange : IEnumerable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CellCount](../../aspose.cells/unionrange/cellcount/) { get; } | Obtiene el recuento total de celdas en el rango. |
| [ColumnCount](../../aspose.cells/unionrange/columncount/) { get; } | Obtiene el recuento de filas en el rango. |
| [FirstColumn](../../aspose.cells/unionrange/firstcolumn/) { get; } | Obtiene el índice de la primera columna del rango. |
| [FirstRow](../../aspose.cells/unionrange/firstrow/) { get; } | Obtiene el índice de la primera fila del rango. |
| [HasRange](../../aspose.cells/unionrange/hasrange/) { get; } | Indica si esto tiene rango. |
| [Hyperlinks](../../aspose.cells/unionrange/hyperlinks/) { get; } | Obtiene todos los hipervínculos en el rango. |
| [Name](../../aspose.cells/unionrange/name/) { get; set; } | Obtiene o establece el nombre del rango. |
| [RangeCount](../../aspose.cells/unionrange/rangecount/) { get; } | Obtiene la cantidad de los rangos. |
| [Ranges](../../aspose.cells/unionrange/ranges/) { get; } | Obtiene todos los rangos de unión. |
| [RefersTo](../../aspose.cells/unionrange/refersto/) { get; } | Obtiene a qué se refiere el rango. |
| [RowCount](../../aspose.cells/unionrange/rowcount/) { get; } | Obtiene el recuento de filas en el rango. |
| [Value](../../aspose.cells/unionrange/value/) { get; set; } | Obtiene y establece los valores del rango. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ApplyStyle](../../aspose.cells/unionrange/applystyle/)(Style, StyleFlag) | Aplica formatos a todo un rango. |
| [Copy](../../aspose.cells/unionrange/copy/)(UnionRange, PasteOptions) | Copiando el rango con opciones de pegado especial. |
| [GetEnumerator](../../aspose.cells/unionrange/getenumerator/)() | Obtiene el enumerador de celdas en este Rango. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect)(Range[]) | Interseca otro rango. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_2)(string) | Interseca otro rango. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_1)(UnionRange) | Interseca otro rango. |
| [Merge](../../aspose.cells/unionrange/merge/)() | Combina un rango de celdas en una sola celda. |
| [PutValue](../../aspose.cells/unionrange/putvalue/)(string, bool, bool) | Inserta un valor en el rango; si es apropiado, el valor se convertirá a otro tipo de datos y se restablecerá el formato numérico de la celda. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders)(CellBorderType, Color) | Establece los bordes exteriores alrededor de un rango de celdas con el mismo estilo y color de borde. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders_1)(CellBorderType[], Color[]) | Establece bordes externos alrededor de un rango de celdas. |
| [SetStyle](../../aspose.cells/unionrange/setstyle/)(Style) | Establece el estilo del rango. |
| [Union](../../aspose.cells/unionrange/union/#union)(Range[]) | Une los rangos. |
| [Union](../../aspose.cells/unionrange/union/#union_2)(string) | Une otro rango. |
| [Union](../../aspose.cells/unionrange/union/#union_1)(UnionRange) | Une otro rango. |
| [UnMerge](../../aspose.cells/unionrange/unmerge/)() | Descombina celdas combinadas de este rango. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassUnionRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un rango de unión usando la API correcta
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A10,C1:C10", 0);
            
            // Establece el valor para todo el rango de unión
            unionRange.Value = "Test";
            
            // Aplica estilo al rango de unión
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // Guarda el libro de trabajo
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


