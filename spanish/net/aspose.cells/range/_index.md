---
title: Range
second_title: Referencia de API de Aspose.Cells para .NET
description: Encapsula el objeto que representa un rango de celdas dentro de una hoja de cálculo.
type: docs
weight: 5030
url: /es/net/aspose.cells/range/
---
## Range class

Encapsula el objeto que representa un rango de celdas dentro de una hoja de cálculo.

```csharp
public class Range
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Address](../../aspose.cells/range/address) { get; } | Obtiene la dirección del rango. |
| [ColumnCount](../../aspose.cells/range/columncount) { get; } | Obtiene el conteo de columnas en el rango. |
| [ColumnWidth](../../aspose.cells/range/columnwidth) { get; set; } | Establece u obtiene el ancho de columna de este rango |
| [CurrentRegion](../../aspose.cells/range/currentregion) { get; } | Devuelve un objeto Range que representa la región actual. La región actual es un rango delimitado por cualquier combinación de filas y columnas en blanco. |
| [EntireColumn](../../aspose.cells/range/entirecolumn) { get; } | Obtiene un objeto Range que representa la columna (o columnas) completa que contiene el rango especificado. |
| [EntireRow](../../aspose.cells/range/entirerow) { get; } | Obtiene un objeto Range que representa toda la fila (o filas) que contiene el rango especificado. |
| [FirstColumn](../../aspose.cells/range/firstcolumn) { get; } | Obtiene el índice de la primera columna del rango. |
| [FirstRow](../../aspose.cells/range/firstrow) { get; } | Obtiene el índice de la primera fila del rango. |
| [Height](../../aspose.cells/range/height) { get; } | Obtiene el ancho de un rango en puntos. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks) { get; } | Obtiene todos los hipervínculos en el rango. |
| [Item](../../aspose.cells/range/item) { get; } | Obtiene[`Cell`](../cell) objeto en este rango. |
| [Left](../../aspose.cells/range/left) { get; } | Obtiene la distancia, en puntos, desde el borde izquierdo de la columna A hasta el borde izquierdo del rango. |
| [Name](../../aspose.cells/range/name) { get; set; } | Obtiene o establece el nombre del rango. |
| [RefersTo](../../aspose.cells/range/refersto) { get; } | Obtiene las referencias del rango. |
| [RowCount](../../aspose.cells/range/rowcount) { get; } | Obtiene el conteo de filas en el rango. |
| [RowHeight](../../aspose.cells/range/rowheight) { get; set; } | Establece u obtiene la altura de las filas en este rango |
| [Top](../../aspose.cells/range/top) { get; } | Obtiene la distancia, en puntos, desde el borde superior de la fila 1 hasta el borde superior del rango. |
| [Value](../../aspose.cells/range/value) { get; set; } | Obtiene y establece el valor del rango. |
| [Width](../../aspose.cells/range/width) { get; } | Obtiene el ancho de un rango en puntos. |
| [Worksheet](../../aspose.cells/range/worksheet) { get; } | Obtiene el[`Worksheet`](./worksheet) objeto que contiene este rango. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ApplyStyle](../../aspose.cells/range/applystyle)(Style, StyleFlag) | Aplica formatos para todo un rango. |
| [AutoFill](../../aspose.cells/range/autofill#autofill)(Range) | Completa automáticamente el rango objetivo. |
| [AutoFill](../../aspose.cells/range/autofill#autofill_1)(Range, AutoFillType) | Completa automáticamente el rango objetivo. |
| [Copy](../../aspose.cells/range/copy#copy)(Range) | Copia datos (incluidas fórmulas), formato, objetos de dibujo, etc. de un rango de origen. |
| [Copy](../../aspose.cells/range/copy#copy_1)(Range, PasteOptions) | Copiando el rango con opciones especiales de pegado. |
| [CopyData](../../aspose.cells/range/copydata)(Range) | Copia datos de celda (incluidas fórmulas) de un rango de origen. |
| [CopyStyle](../../aspose.cells/range/copystyle)(Range) | Copia la configuración de estilo de un rango de origen. |
| [CopyValue](../../aspose.cells/range/copyvalue)(Range) | Copia el valor de la celda de un rango de origen. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable)() | Exporta datos en este rango a unDataTable objeto. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable_1)(ExportTableOptions) | Exporta datos en este rango a unDataTable objeto. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring)() | Exporta datos en este rango a unDataTable objeto. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull)(int, int) | Obtiene[`Cell`](../cell) objeto o nulo en este rango. |
| [GetEnumerator](../../aspose.cells/range/getenumerator)() | Obtiene el enumerador de las celdas de este rango. |
| [GetOffset](../../aspose.cells/range/getoffset)(int, int) | Obtiene[`Range`](../range) rango por desplazamiento. |
| [Intersect](../../aspose.cells/range/intersect)(Range) | Devuelve un[`Range`](../range) objeto que representa la intersección rectangular de dos rangos. |
| [IsIntersect](../../aspose.cells/range/isintersect)(Range) | Indica si el rango es intersección. |
| [Merge](../../aspose.cells/range/merge)() | Combina un rango de celdas en una sola celda. |
| [MoveTo](../../aspose.cells/range/moveto)(int, int) | Mueve el rango actual al rango dest. |
| [PutValue](../../aspose.cells/range/putvalue)(string, bool, bool) | Pone un valor en el rango, si corresponde, el valor se convertirá a otro tipo de datos y se restablecerá el formato de número de celda. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders)(BorderType, CellBorderType, CellsColor) | Establecer dentro de los límites del rango. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder)(BorderType, CellBorderType, Color) | Establece el borde del contorno alrededor de un rango de celdas. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders)(CellBorderType, Color) | Establece los bordes del contorno alrededor de un rango de celdas con el mismo estilo y color de borde. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders_1)(CellBorderType[], Color[]) | Establece bordes de línea alrededor de un rango de celdas. |
| [SetStyle](../../aspose.cells/range/setstyle)(Style) | Establece el estilo del rango. |
| override [ToString](../../aspose.cells/range/tostring)() | Devuelve una cadena que representa el objeto Range actual. |
| [Union](../../aspose.cells/range/union)(Range) | Devuelve la unión de dos rangos. |
| [UnMerge](../../aspose.cells/range/unmerge)() | Separa las celdas combinadas de este rango. |

### Ejemplos

```csharp

[C#]

// Instanciando un objeto Workbook
Workbook workbook = new Workbook();
// Obtenga las primeras celdas de la hoja de trabajo.
Cells cells = workbook.Worksheets[0].Cells;
// Crea un rango (A1:D3).
Range range = cells.CreateRange("A1", "D3");
// Establecer valor en el rango.
range.Value = "Hello";
//Guardar el archivo Excel
workbook.Save("book1.xlsm");

 [Visual Basic]

'Crear una instancia de un objeto Workbook
Dim workbook As Workbook = New Workbook()
'Obtenga las primeras celdas de la hoja de trabajo.
Dim cells as Cells = workbook.Worksheets[0].Cells
'Cree un rango (A1:D3).
Dim range as Range = cells.CreateRange("A1", "D3")
'Establezca el valor en el rango.
range.Value = "Hello"
'Guarde el archivo de Excel
workbook.Save("book1.xlsm")
```

### Ver también

* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
