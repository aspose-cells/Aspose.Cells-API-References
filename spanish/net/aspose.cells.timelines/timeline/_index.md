---
title: "Clase Timeline"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Timelines.Timeline. Descripción resumida de la vista de Línea de tiempo debido a que MS Excel 2003 no admite Línea de tiempo"
type: docs
url: /es/net/aspose.cells.timelines/timeline/
---
## Timeline class

Descripción resumida de la vista de línea de tiempo. Debido a MS Excel, Excel 2003 no admite la línea de tiempo.

```csharp
public class Timeline
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Caption](../../aspose.cells.timelines/timeline/caption/) { get; set; } | Obtiene o establece el título de esta Línea de tiempo. |
| [CurrentLevel](../../aspose.cells.timelines/timeline/currentlevel/) { get; set; } | El nivel de tiempo actual de la Línea de tiempo. |
| [HeightPixel](../../aspose.cells.timelines/timeline/heightpixel/) { get; set; } | (**Obsolete.**) Devuelve o establece la altura de la línea de tiempo especificada, en píxeles. |
| [LeftPixel](../../aspose.cells.timelines/timeline/leftpixel/) { get; set; } | (**Obsolete.**) Devuelve o establece el desplazamiento horizontal de la forma de la línea de tiempo desde su columna izquierda, en píxeles. |
| [Name](../../aspose.cells.timelines/timeline/name/) { get; set; } | Devuelve o establece el nombre de la Línea de tiempo especificada |
| [SelectionLevel](../../aspose.cells.timelines/timeline/selectionlevel/) { get; set; } | Obtiene y establece el nivel de tiempo en el que se realizó la selección actual para la Línea de tiempo. |
| [Shape](../../aspose.cells.timelines/timeline/shape/) { get; } | Devuelve el objeto [`TimelineShape`](../../aspose.cells.drawing/timelineshape/) asociado a esta Línea de tiempo. |
| [ShowHeader](../../aspose.cells.timelines/timeline/showheader/) { get; set; } | Indica si se debe mostrar el encabezado de esta línea de tiempo. |
| [ShowHorizontalScrollbar](../../aspose.cells.timelines/timeline/showhorizontalscrollbar/) { get; set; } | Indica si se debe mostrar la barra de desplazamiento horizontal. |
| [ShowSelectionLabel](../../aspose.cells.timelines/timeline/showselectionlabel/) { get; set; } | Indica si se debe mostrar la etiqueta de selección. |
| [ShowTimeLevel](../../aspose.cells.timelines/timeline/showtimelevel/) { get; set; } | Indica si se debe mostrar el cuadro de selección desplegable del nivel de tiempo. |
| [StartDate](../../aspose.cells.timelines/timeline/startdate/) { get; set; } | Obtiene y establece la fecha de inicio de la posición de desplazamiento del intervalo de tiempo de este `Timeline`. |
| [TopPixel](../../aspose.cells.timelines/timeline/toppixel/) { get; set; } | (**Obsolete.**) Devuelve o establece el desplazamiento vertical de la forma de la línea de tiempo desde su fila superior, en píxeles. |
| [WidthPixel](../../aspose.cells.timelines/timeline/widthpixel/) { get; set; } | (**Obsolete.**) Devuelve o establece el ancho de la línea de tiempo especificada, en píxeles. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetSelectedDateTimeRange](../../aspose.cells.timelines/timeline/getselecteddatetimerange/)() | Obtiene el rango seleccionado de fecha y hora. |
| [Select](../../aspose.cells.timelines/timeline/select/)(DateTime, DateTime, bool) | Selecciona el elemento entre la fecha y hora. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using Aspose.Cells.Timelines;
    using System;

    public class TimelineDemo
    {
        public static void TimelineExample()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Rellena la hoja de cálculo con datos de ejemplo
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";

            // Crear estilo de fecha
            Style dateStyle = new CellsFactory().CreateStyle();
            dateStyle.Custom = "m/d/yyyy";
            cells[0, 1].Value = "date";
            cells[1, 1].Value = new DateTime(2021, 2, 5);
            cells[2, 1].Value = new DateTime(2022, 3, 8);
            cells[3, 1].Value = new DateTime(2023, 4, 10);
            cells[4, 1].Value = new DateTime(2024, 5, 16);
            // Establecer estilo de fecha
            cells[1, 1].SetStyle(dateStyle);
            cells[2, 1].SetStyle(dateStyle);
            cells[3, 1].SetStyle(dateStyle);
            cells[4, 1].SetStyle(dateStyle);

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;

            // Agregar una tabla dinámica
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C5", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "date");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Actualizar los datos de la tabla dinámica
            pivot.RefreshData();
            pivot.CalculateData();

            // Agregar una nueva Línea de tiempo usando una tabla dinámica como fuente de datos
            sheet.Timelines.Add(pivot, 10, 5, "date");

            // Obtener objeto Timeline
            Timeline timelineObj = sheet.Timelines[0];

            // Establecer propiedades de la Línea de tiempo
            timelineObj.Caption = "timeline caption test";
            timelineObj.Name = "timeline name test";
            timelineObj.LeftPixel = 100;
            timelineObj.TopPixel = 50;
            timelineObj.WidthPixel = 300;
            timelineObj.HeightPixel = 100;

            // Guarda el libro de trabajo
            book.Save("TimelineExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Timelines](../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../)


