---
title: "Clase IconFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.IconFilter. Representa un filtro de iconos"
type: docs
url: /es/net/aspose.cells/iconfilter/
---
## IconFilter class

Representa el filtro de iconos.

```csharp
public class IconFilter
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [IconId](../../aspose.cells/iconfilter/iconid/) { get; set; } | Obtiene y establece el índice basado en cero de un icono en un conjunto de iconos. |
| [IconSetType](../../aspose.cells/iconfilter/iconsettype/) { get; set; } | Obtiene y establece qué conjunto de iconos se usa para este criterio de filtro. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassIconFilterDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Rellene datos de ejemplo
                for (int i = 0; i < 10; i++)
                {
                    worksheet.Cells[i, 0].PutValue(i * 10);
                }

                // Cree filtro automático
                worksheet.AutoFilter.Range = "A1:A10";
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.IconFilter;

                // Obtenga el filtro de iconos
                IconFilter iconFilter = (IconFilter)filterColumn.Filter;

                // Establezca propiedades del filtro de iconos
                iconFilter.IconSetType = IconSetType.Arrows3;
                iconFilter.IconId = 1; // Filter for middle arrow

                Console.WriteLine($"IconFilter created with IconSetType: {iconFilter.IconSetType} and IconId: {iconFilter.IconId}");

                // Guarda el libro de trabajo
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon filter applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with IconFilter: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


