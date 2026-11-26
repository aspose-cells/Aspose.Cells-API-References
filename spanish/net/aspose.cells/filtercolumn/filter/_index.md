---
title: "FilterColumn.Filter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FilterColumn. Obtiene y establece la condición de filtrado de datos"
type: docs
url: /es/net/aspose.cells/filtercolumn/filter/
---
## FilterColumn.Filter property

Obtiene y establece la condición de filtrado de datos.

```csharp
[Obsolete("Use corresponding property according to the filter type instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Filter { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad correspondiente según [`FilterType`](../filtertype/). Y para el tipo de filtro MultipleFilters, el objeto devuelto es ahora [`FilterValueCollection`](../../filtervaluecollection/) en lugar de [`MultipleFilterCollection`](../../multiplefiltercollection/). Esta propiedad será eliminada 12 meses después, a partir de octubre de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFilterDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo con formato de color
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Color");
            cells["A2"].PutValue("Red");
            cells["A3"].PutValue("Red");
            cells["A4"].PutValue("Blue");
            
            // Formatear celdas con colores
            Style redStyle = workbook.CreateStyle();
            redStyle.ForegroundColor = Color.Red;
            redStyle.Pattern = BackgroundType.Solid;
            
            Style blueStyle = workbook.CreateStyle();
            blueStyle.ForegroundColor = Color.Blue;
            blueStyle.Pattern = BackgroundType.Solid;
            
            cells["A2"].SetStyle(redStyle);
            cells["A3"].SetStyle(redStyle);
            cells["A4"].SetStyle(blueStyle);
            
            // Aplicar filtro automático
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Agregar filtro de color para celdas rojas
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // Acceder a la columna de filtro y su propiedad Filter
            FilterColumn fc = filter.FilterColumns[0];
            ColorFilter cf = fc.Filter as ColorFilter;
            
            // Mostrar propiedades del filtro
            Console.WriteLine($"Filter type: {fc.FilterType}");
            Console.WriteLine($"Filter by fill color: {cf.FilterByFillColor}");
            Console.WriteLine($"Filter color: {cf.GetColor(workbook.Worksheets)}");
            
            // Guarda el libro de trabajo
            workbook.Save("ColorFilterDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


