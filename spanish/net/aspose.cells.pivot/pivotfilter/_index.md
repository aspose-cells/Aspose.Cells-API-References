---
title: "Clase PivotFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotFilter. Representa un PivotFilter en la colección PivotFilter"
type: docs
url: /es/net/aspose.cells.pivot/pivotfilter/
---
## PivotFilter class

Representa un PivotFilter en la colección PivotFilter.

```csharp
public class PivotFilter
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoFilter](../../aspose.cells.pivot/pivotfilter/autofilter/) { get; } | (**Obsolete.**) Obtiene el autofiltro del filtro dinámico. |
| [EvaluationOrder](../../aspose.cells.pivot/pivotfilter/evaluationorder/) { get; set; } | Obtiene el orden de evaluación del filtro dinámico. |
| [FieldIndex](../../aspose.cells.pivot/pivotfilter/fieldindex/) { get; } | Obtiene el índice del campo origen al que se aplica este filtro dinámico. |
| [FilterCategory](../../aspose.cells.pivot/pivotfilter/filtercategory/) { get; } | Obtiene la categoría de este filtro. |
| [FilterType](../../aspose.cells.pivot/pivotfilter/filtertype/) { get; } | Obtiene el tipo de filtro del filtro dinámico. |
| [MeasureCubeFieldIndex](../../aspose.cells.pivot/pivotfilter/measurecubefieldindex/) { get; } | Especifica el índice del campo de cubo de medida. Esta propiedad se usa solo en filtros de pivotes OLAP y especifica en qué medida debe aplicarse un filtro de valor. |
| [MeasureFldIndex](../../aspose.cells.pivot/pivotfilter/measurefldindex/) { get; set; } | (**Obsolete.**) Obtiene el índice del campo de medida del filtro dinámico. |
| [MemberPropertyFieldIndex](../../aspose.cells.pivot/pivotfilter/memberpropertyfieldindex/) { get; set; } | Obtiene el índice del campo de propiedad de miembro del filtro dinámico. |
| [Name](../../aspose.cells.pivot/pivotfilter/name/) { get; set; } | Obtiene el nombre del filtro dinámico. |
| [UseWholeDay](../../aspose.cells.pivot/pivotfilter/usewholeday/) { get; set; } | Indica si se deben usar días completos en sus criterios de filtrado de fechas. |
| [Value1](../../aspose.cells.pivot/pivotfilter/value1/) { get; set; } | Obtiene el valor de cadena 1 del filtro dinámico de etiqueta. |
| [Value2](../../aspose.cells.pivot/pivotfilter/value2/) { get; set; } | Obtiene el valor de cadena 2 del filtro dinámico de etiqueta. |
| [ValueFieldIndex](../../aspose.cells.pivot/pivotfilter/valuefieldindex/) { get; set; } | Obtiene el índice del campo de valor en la región de valores. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetDateTimeValues](../../aspose.cells.pivot/pivotfilter/getdatetimevalues/)() | Obtiene los valores del filtro numérico. |
| [GetLabels](../../aspose.cells.pivot/pivotfilter/getlabels/)() | Obtiene las etiquetas del filtro de título. |
| [GetNumberValues](../../aspose.cells.pivot/pivotfilter/getnumbervalues/)() | Obtiene los valores del filtro numérico. |
| [GetTop10Value](../../aspose.cells.pivot/pivotfilter/gettop10value/)() | Obtiene la configuración de los 10 principales del filtro. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterDemo
    {
        public static void PivotFilterExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Rellena la hoja de cálculo con datos de ejemplo
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Agregar una tabla dinámica a la hoja de cálculo
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Establecer estilo de tabla pivot
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Agregar un filtro de tabla dinámica
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Establecer propiedades adicionales para el filtro de tabla dinámica
            filter.Value1 = "SampleValue1";
            filter.Value2 = "SampleValue2";
            filter.MeasureFldIndex = 1;
            filter.MemberPropertyFieldIndex = 2;
            filter.Name = "SampleFilter";
            filter.EvaluationOrder = 1;

            // Actualizar y calcular los datos de la tabla dinámica
            pivot.RefreshData();
            pivot.CalculateData();

            // Guarda el libro de trabajo
            book.Save("PivotFilterExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


