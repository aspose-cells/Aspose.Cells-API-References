---
title: "Clase Range"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Range. Encapsula el objeto que representa un rango de celdas dentro de una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/range/
---
## Range class

Encapsula el objeto que representa un rango de celdas dentro de una hoja de cálculo.

```csharp
public class Range : IEnumerable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Range](range/#constructor)(CellArea, Cells) | Constructor de la clase. |
| [Range](range/#constructor_1)(int, int, int, int, Cells) | Constructor de la clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Address](../../aspose.cells/range/address/) { get; } | Obtiene la dirección del rango. |
| [ColumnCount](../../aspose.cells/range/columncount/) { get; } | Obtiene el recuento de columnas en el rango. |
| [ColumnWidth](../../aspose.cells/range/columnwidth/) { get; set; } | Establece u obtiene el ancho de columna de este rango |
| [CurrentRegion](../../aspose.cells/range/currentregion/) { get; } | Devuelve un objeto Range que representa la región actual. La región actual es un rango delimitado por cualquier combinación de filas en blanco y columnas en blanco. |
| [EntireColumn](../../aspose.cells/range/entirecolumn/) { get; } | Obtiene un objeto Range que representa la columna completa (o columnas) que contiene el rango especificado. |
| [EntireRow](../../aspose.cells/range/entirerow/) { get; } | Obtiene un objeto Range que representa la fila completa (o filas) que contiene el rango especificado. |
| [FirstColumn](../../aspose.cells/range/firstcolumn/) { get; } | Obtiene el índice de la primera columna del rango. |
| [FirstRow](../../aspose.cells/range/firstrow/) { get; } | Obtiene el índice de la primera fila del rango. |
| [Height](../../aspose.cells/range/height/) { get; } | Obtiene el ancho de un rango en puntos. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks/) { get; } | Obtiene todos los hipervínculos en el rango. |
| [Item](../../aspose.cells/range/item/) { get; } | Obtiene el objeto [`Cell`](../cell/) en este rango. |
| [Left](../../aspose.cells/range/left/) { get; } | Obtiene la distancia, en puntos, desde el borde izquierdo de la columna A hasta el borde izquierdo del rango. |
| [Name](../../aspose.cells/range/name/) { get; set; } | Obtiene o establece el nombre del rango. |
| [RefersTo](../../aspose.cells/range/refersto/) { get; } | Obtiene a qué se refiere el rango. |
| [RowCount](../../aspose.cells/range/rowcount/) { get; } | Obtiene el recuento de filas en el rango. |
| [RowHeight](../../aspose.cells/range/rowheight/) { get; set; } | Establece u obtiene la altura de las filas en este rango |
| [Top](../../aspose.cells/range/top/) { get; } | Obtiene la distancia, en puntos, desde el borde superior de la fila 1 hasta el borde superior del rango. |
| [Value](../../aspose.cells/range/value/) { get; set; } | Obtiene y establece el valor del rango. |
| [Width](../../aspose.cells/range/width/) { get; } | Obtiene el ancho de un rango en puntos. |
| [Worksheet](../../aspose.cells/range/worksheet/) { get; } | Obtiene el objeto [`Worksheet`](./worksheet/) que contiene este rango. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddHyperlink](../../aspose.cells/range/addhyperlink/)(string, string, string) | Agrega un hipervínculo a una celda especificada o a un rango de celdas. |
| [ApplyStyle](../../aspose.cells/range/applystyle/)(Style, StyleFlag) | Aplica formatos a todo un rango. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill)(Range) | Rellena automáticamente el rango objetivo. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill_1)(Range, AutoFillType) | Rellena automáticamente el rango objetivo. |
| [Clear](../../aspose.cells/range/clear/)() | Borra este rango. |
| [ClearComments](../../aspose.cells/range/clearcomments/)() | Borra los comentarios de este rango. |
| [ClearContents](../../aspose.cells/range/clearcontents/)() | Borra el contenido de este rango. |
| [ClearFormats](../../aspose.cells/range/clearformats/)() | Borra los formatos de este rango. |
| [ClearHyperlinks](../../aspose.cells/range/clearhyperlinks/)(bool) | Solo elimina hipervínculos. |
| [Copy](../../aspose.cells/range/copy/#copy)(Range) | Copia datos (incluidas fórmulas), formato, objetos de dibujo, etc., de un rango de origen. |
| [Copy](../../aspose.cells/range/copy/#copy_1)(Range, PasteOptions) | Copiando el rango con opciones de pegado especial. |
| [CopyData](../../aspose.cells/range/copydata/)(Range) | Copia datos de celda (incluidas fórmulas) de un rango de origen. |
| [CopyStyle](../../aspose.cells/range/copystyle/)(Range) | Copia la configuración de estilo de un rango de origen. |
| [CopyValue](../../aspose.cells/range/copyvalue/)(Range) | Copia el valor de la celda de un rango de origen. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable)() | Exporta los datos de este rango a un objeto DataTable. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable_1)(ExportTableOptions) | Exporta los datos de este rango a un objeto DataTable. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring/)() | Exporta los datos de este rango a un objeto DataTable. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull/)(int, int) | Obtiene el objeto [`Cell`](../cell/) o null en este rango. |
| [GetEnumerator](../../aspose.cells/range/getenumerator/)() | Obtiene el enumerador de celdas en este Rango. |
| [GetOffset](../../aspose.cells/range/getoffset/)(int, int) | Obtiene el rango `Range` por desplazamiento. |
| [Intersect](../../aspose.cells/range/intersect/)(Range) | Devuelve un objeto `Range` que representa la intersección rectangular de dos rangos. |
| [IsBlank](../../aspose.cells/range/isblank/)() | Indica si el rango contiene valores. |
| [IsIntersect](../../aspose.cells/range/isintersect/)(Range) | Indica si el rango está intersectado. |
| [Merge](../../aspose.cells/range/merge/)() | Combina un rango de celdas en una sola celda. |
| [MoveTo](../../aspose.cells/range/moveto/)(int, int) | Mueve el rango actual al rango de destino. |
| [PutValue](../../aspose.cells/range/putvalue/)(string, bool, bool) | Inserta un valor en el rango; si es apropiado, el valor se convertirá a otro tipo de datos y se restablecerá el formato numérico de la celda. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders/)(BorderType, CellBorderType, CellsColor) | Establece los bordes internos del rango. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder)(BorderType, CellBorderType, CellsColor) | Establece el borde exterior alrededor de un rango de celdas. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder_1)(BorderType, CellBorderType, Color) | Establece el borde exterior alrededor de un rango de celdas. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | Establece los bordes exteriores alrededor de un rango de celdas con el mismo estilo y color de borde. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | Establece los bordes exteriores alrededor de un rango de celdas con el mismo estilo y color de borde. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_2)(CellBorderType[], Color[]) | Establece bordes externos alrededor de un rango de celdas. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle)(Style) | Establece el estilo del rango. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle_1)(Style, bool) | Aplicar el estilo de celda. |
| [ToHtml](../../aspose.cells/range/tohtml/)(HtmlSaveOptions) | Convertir el rango a html. |
| [ToImage](../../aspose.cells/range/toimage/)(ImageOrPrintOptions) | Convierte el rango a imagen. |
| [ToJson](../../aspose.cells/range/tojson/)(JsonSaveOptions) | Convertir el rango a valor JSON. |
| override [ToString](../../aspose.cells/range/tostring/)() | Devuelve una cadena que representa el objeto Range actual. |
| [Transpose](../../aspose.cells/range/transpose/)() | Transponer (rotar) datos de filas a columnas o viceversa. |
| [Union](../../aspose.cells/range/union/)(Range) | (**Obsolete.**) Devuelve la unión de dos rangos. |
| [UnionRang](../../aspose.cells/range/unionrang/)(Range) | (**Obsolete.**) Devuelve el resultado de la unión de dos rangos. |
| [UnionRanges](../../aspose.cells/range/unionranges/)(Range[]) | Devuelve el resultado de la unión de dos rangos. |
| [UnMerge](../../aspose.cells/range/unmerge/)() | Descombina celdas combinadas de este rango. |

### Observaciones

La clase Range denota una región de la hoja de cálculo de Excel. Con ella, puedes dar formato y establecer el valor del rango. Y también puedes copiar fácilmente rangos de Excel.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "D3");
            range.Value = "Hello";
            workbook.Save("book1.xlsm");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


