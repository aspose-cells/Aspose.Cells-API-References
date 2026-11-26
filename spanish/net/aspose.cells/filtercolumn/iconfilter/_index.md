---
title: "FilterColumn.IconFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FilterColumn. Obtiene IconFilter para filtrar datos por ícono"
type: docs
url: /es/net/aspose.cells/filtercolumn/iconfilter/
---
## FilterColumn.IconFilter property

Obtiene `IconFilter` para filtrar datos por ícono.

```csharp
public IconFilter IconFilter { get; }
```

### Observaciones

Antes de usar esta propiedad, asegúrese de que [`FilterType`](../filtertype/) sea IconFilter, de lo contrario se devolverá null.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyIconFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Agregar datos de muestra con formato condicional que usa íconos
                worksheet.Cells["A1"].PutValue("Performance");
                worksheet.Cells["A2"].PutValue(85);
                worksheet.Cells["A3"].PutValue(72);
                worksheet.Cells["A4"].PutValue(93);
                worksheet.Cells["A5"].PutValue(65);

                // Aplicar filtro automático al rango
                worksheet.AutoFilter.Range = "A1:A5";

                // Obtener la columna de filtro
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Acceder a la propiedad IconFilter (solo lectura)
                IconFilter iconFilter = filterColumn.IconFilter;

                // Mostrar propiedades de IconFilter si existe
                if (iconFilter != null)
                {
                    Console.WriteLine("IconFilter is available");
                    Console.WriteLine($"IconSetType: {iconFilter.IconSetType}");
                    Console.WriteLine($"IconId: {iconFilter.IconId}");
                }
                else
                {
                    Console.WriteLine("No IconFilter is currently applied to this column");
                }

                // Guarda el libro de trabajo
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("IconFilter demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [IconFilter](../../iconfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


