---
title: "Clase ListObject"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Tables.ListObject. Representa una tabla en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells.tables/listobject/
---
## ListObject class

Representa una tabla en una hoja de cálculo.

```csharp
public class ListObject
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription/) { get; set; } | Obtiene y establece la descripción alternativa. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext/) { get; set; } | Obtiene y establece el texto alternativo. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter/) { get; } | Obtiene el filtro automático de esta tabla. |
| [Comment](../../aspose.cells.tables/listobject/comment/) { get; set; } | Obtiene y establece el comentario de la tabla. |
| [DataRange](../../aspose.cells.tables/listobject/datarange/) { get; } | Obtiene el rango de datos de la Tabla. |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype/) { get; } | Obtiene el tipo de origen de datos de la tabla. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname/) { get; set; } | Obtiene y establece el nombre para mostrar de la tabla. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn/) { get; } | Obtiene la columna final del rango. |
| [EndRow](../../aspose.cells.tables/listobject/endrow/) { get; } | Obtiene la fila final del rango. |
| [HasAutoFilter](../../aspose.cells.tables/listobject/hasautofilter/) { get; set; } | Indica si el filtro automático se aplica a esta tabla. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns/) { get; } | Obtiene la lista de [`ListColumn`](../listcolumn/) de esta tabla. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable/) { get; } | Obtiene la QueryTable vinculada. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow/) { get; set; } | Obtiene y establece si esta Tabla muestra la fila de encabezado. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes/) { get; set; } | Indica si se aplica formato de franjas de columna. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn/) { get; set; } | Indica si la primera columna de la tabla tiene el estilo aplicado. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn/) { get; set; } | Indica si la última columna de la tabla tiene el estilo aplicado. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes/) { get; set; } | Indica si se aplica formato de franjas de fila. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals/) { get; set; } | Obtiene y establece si esta TAble muestra la fila total. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn/) { get; } | Obtiene la columna inicial del rango. |
| [StartRow](../../aspose.cells.tables/listobject/startrow/) { get; } | Obtiene la fila inicial del rango. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename/) { get; set; } | Obtiene y establece el nombre del estilo de tabla |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype/) { get; set; } | Obtiene y el estilo de tabla incorporado. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap/) { get; } | Obtiene un [`XmlMap`](./xmlmap/) usado para esta lista. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange/)() | Aplica el estilo de tabla al rango. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange)() | Convierte la tabla a rango. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange_1)(TableToRangeOptions) | Convierte la tabla a rango. |
| [Filter](../../aspose.cells.tables/listobject/filter/)() | (**Obsoleto.**) Filtra la tabla. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula)(int, int, string) | Coloca la fórmula en la celda de la tabla. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula_1)(int, int, string, bool) | Coloca la fórmula en la celda de la tabla. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue)(int, int, object) | Coloca el valor en la celda. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue_1)(int, int, object, bool) | Coloca el valor en la celda. |
| [RemoveAutoFilter](../../aspose.cells.tables/listobject/removeautofilter/)() | Elimina el filtro automático que se aplica a esta tabla. |
| [Resize](../../aspose.cells.tables/listobject/resize/)(int, int, int, int, bool) | Redimensiona el rango del objeto de lista. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname/)() | Actualiza el nombre de todas las columnas de lista a las celdas en la tabla. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectDemo
    {
        public static void ListObjectExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Poblar la hoja de cálculo con algunos datos
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Agregar un ListObject (tabla) a la hoja de cálculo
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Establece algunas propiedades del ListObject
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;
            table.DisplayName = "SampleTable";
            table.Comment = "This is a sample table.";
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.ShowTableStyleRowStripes = true;
            table.ShowTableStyleColumnStripes = true;
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Guarda el libro de trabajo
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


