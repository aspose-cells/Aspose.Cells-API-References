---
title: "Clase AutoFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.AutoFilter. Representa el autofiltro para la hoja de cálculo especificada"
type: docs
url: /es/net/aspose.cells/autofilter/
---
## AutoFilter class

Representa el autofiltro para la hoja de cálculo especificada.

```csharp
public class AutoFilter
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FilterColumns](../../aspose.cells/autofilter/filtercolumns/) { get; } | Obtiene la colección de columnas de filtro. |
| [Range](../../aspose.cells/autofilter/range/) { get; set; } | Representa el rango al que se aplica el AutoFilter especificado. |
| [ShowFilterButton](../../aspose.cells/autofilter/showfilterbutton/) { get; set; } | Indica si el botón AutoFilter para esta columna es visible. |
| [Sorter](../../aspose.cells/autofilter/sorter/) { get; } | Obtiene el ordenador de datos. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddDateFilter](../../aspose.cells/autofilter/adddatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Añade un filtro de fecha. |
| [AddFillColorFilter](../../aspose.cells/autofilter/addfillcolorfilter/)(int, BackgroundType, CellsColor, CellsColor) | Añade un filtro de color de relleno. |
| [AddFilter](../../aspose.cells/autofilter/addfilter/)(int, string) | Añade un filtro para una columna de filtro. |
| [AddFontColorFilter](../../aspose.cells/autofilter/addfontcolorfilter/)(int, CellsColor) | Añade un filtro de color de fuente. |
| [AddIconFilter](../../aspose.cells/autofilter/addiconfilter/)(int, IconSetType, int) | Añade un filtro de icono. |
| [Custom](../../aspose.cells/autofilter/custom/#custom)(int, FilterOperatorType, object) | Filtra una lista con un criterio personalizado. |
| [Custom](../../aspose.cells/autofilter/custom/#custom_1)(int, FilterOperatorType, object, bool, FilterOperatorType, object) | Filtra una lista con criterios personalizados. |
| [DynamicFilter](../../aspose.cells/autofilter/dynamicfilter/)(int, DynamicFilterType) | Añade un filtro dinámico. |
| [Filter](../../aspose.cells/autofilter/filter/)(int, string) | Filtra una lista con criterios especificados. |
| [FilterTop10](../../aspose.cells/autofilter/filtertop10/)(int, bool, bool, int) | Filtrar los 10 elementos principales de la lista |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea)() | Obtiene el [`CellArea`](../cellarea/) donde se aplica este AutoFilter. |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea_1)(bool) | Obtiene el [`CellArea`](../cellarea/) donde se aplica el AutoFilter especificado. |
| [MatchBlanks](../../aspose.cells/autofilter/matchblanks/)(int) | Coincide con todas las celdas en blanco de la lista. |
| [MatchNonBlanks](../../aspose.cells/autofilter/matchnonblanks/)(int) | Coincide con todas las celdas que no están en blanco de la lista. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh)() | Actualiza los autofiltros para ocultar o mostrar las filas. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh_1)(bool) | Obtiene los índices de todas las filas ocultas. |
| [RemoveDateFilter](../../aspose.cells/autofilter/removedatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Elimina un filtro de fecha. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter)(int) | Elimina el filtro específico. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter_1)(int, string) | Elimina un filtro para una columna de filtro. |
| [SetRange](../../aspose.cells/autofilter/setrange/)(int, int, int) | Establece el rango al que se aplica el AutoFilter especificado. |
| [ShowAll](../../aspose.cells/autofilter/showall/)() | Desocultar todas las filas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterDemo
    {
        public static void AutoFilterExample()
        {
            // Creando un flujo de archivo que contiene el archivo Excel que se abrirá
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accediendo a la primera hoja de cálculo en el archivo Excel
            Worksheet worksheet = workbook.Worksheets[0];
            // Creando AutoFilter proporcionando el rango de celdas de la fila de encabezado
            worksheet.AutoFilter.Range = "A1:B8";
            // Filtrando columnas con valores especificados
            worksheet.AutoFilter.Filter(0, "Bananas");
            worksheet.AutoFilter.Refresh();

            // Guardando el archivo Excel modificado.
            workbook.Save("AutoFilterExample.xlsx");
            workbook.Save("AutoFilterExample.pdf");

            // Instanciando un objeto Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accediendo a la primera hoja de cálculo en el archivo Excel
            worksheet = workbook.Worksheets[0];

            // Código adicional para demostrar otras funcionalidades de AutoFilter
            // Estableciendo el rango para AutoFilter
            worksheet.AutoFilter.Range = "A1:B8";
            // Añadiendo un filtro
            worksheet.AutoFilter.AddFilter(0, "Apples");
            // Añadiendo un filtro de fecha
            worksheet.AutoFilter.AddDateFilter(1, DateTimeGroupingType.Year, 2022, 0, 0, 0, 0, 0);

            worksheet.AutoFilter.Refresh();
            // Guardando el archivo Excel modificado.
            workbook.Save("AutoFilterExample2.xlsx");
            workbook.Save("AutoFilterExample2.pdf");

            // Instanciando un objeto Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accediendo a la primera hoja de cálculo en el archivo Excel
            worksheet = workbook.Worksheets[0];
                        
            // Añadiendo un filtro de color de fuente
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Red;

            worksheet.AutoFilter.AddFontColorFilter(0, color);

            worksheet.AutoFilter.Refresh();
            // Guardando el archivo Excel modificado.
            workbook.Save("AutoFilterExample3.xlsx");
            workbook.Save("AutoFilterExample3.pdf");

            // Instanciando un objeto Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accediendo a la primera hoja de cálculo en el archivo Excel
            worksheet = workbook.Worksheets[0];

            // Añadiendo un filtro de color de relleno
            CellsColor foregroundColor = workbook.CreateCellsColor();
            foregroundColor.Color = System.Drawing.Color.Red;
            CellsColor backgroundColor = workbook.CreateCellsColor();
            backgroundColor.Color = System.Drawing.Color.White;

            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, foregroundColor, backgroundColor);

            worksheet.AutoFilter.Refresh();
            // Guardando el archivo Excel modificado.
            workbook.Save("AutoFilterExample4.xlsx");
            workbook.Save("AutoFilterExample4.pdf");

            // Instanciando un objeto Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accediendo a la primera hoja de cálculo en el archivo Excel
            worksheet = workbook.Worksheets[0];

            // Coincidiendo con celdas en blanco
            worksheet.AutoFilter.MatchBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Guardando el archivo Excel modificado.
            workbook.Save("AutoFilterExample5.xlsx");
            workbook.Save("AutoFilterExample5.pdf");

            // Instanciando un objeto Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accediendo a la primera hoja de cálculo en el archivo Excel
            worksheet = workbook.Worksheets[0];

            // Coincidiendo con celdas no en blanco
            worksheet.AutoFilter.MatchNonBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Guardando el archivo Excel modificado.
            workbook.Save("AutoFilterExample6.xlsx");
            workbook.Save("AutoFilterExample6.pdf");

            // Instanciando un objeto Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accediendo a la primera hoja de cálculo en el archivo Excel
            worksheet = workbook.Worksheets[0];

            // Filtro personalizado
            worksheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "Test");

            worksheet.AutoFilter.Refresh();
            // Guardando el archivo Excel modificado.
            workbook.Save("AutoFilterExample7.xlsx");
            workbook.Save("AutoFilterExample7.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


