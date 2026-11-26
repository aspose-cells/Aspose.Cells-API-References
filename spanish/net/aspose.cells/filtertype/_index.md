---
title: "Enumeración FilterType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.FilterType. El tipo de filtro"
type: docs
url: /es/net/aspose.cells/filtertype/
---
## FilterType enumeration

El tipo de filtro.

```csharp
public enum FilterType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| ColorFilter | `0` | Filtrar por color de relleno de la celda. |
| CustomFilters | `1` | Tipo de filtro personalizado. |
| DynamicFilter | `2` | Tipo de filtro dinámico. |
| MultipleFilters | `3` | Cuando se seleccionan varios valores para filtrar, o cuando se elige un grupo de valores de fecha para filtrar, este elemento agrupa esos criterios juntos. |
| IconFilter | `4` | Filtrar por ícono de formato condicional. |
| Top10 | `5` | Filtro Top 10. |
| None | `6` | Sin filtro. |

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFilterTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Color");
            worksheet.Cells["A2"].PutValue("Red");
            worksheet.Cells["A3"].PutValue("Green");
            worksheet.Cells["A4"].PutValue("Blue");
            
            // Cree filtro automático
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Crear filtro de color
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            
            // Agregar filtro de color a la columna
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // Verificar el tipo de filtro
            FilterColumn filterColumn = filter.FilterColumns[0];
            Console.WriteLine("Filter Type: " + filterColumn.FilterType);
            
            // Verificar las propiedades del filtro de color
            if (filterColumn.FilterType == FilterType.ColorFilter)
            {
                ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
                Console.WriteLine("Filter by fill color: " + colorFilter.FilterByFillColor);
                Console.WriteLine("Filter color: " + colorFilter.GetColor(workbook.Worksheets));
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


