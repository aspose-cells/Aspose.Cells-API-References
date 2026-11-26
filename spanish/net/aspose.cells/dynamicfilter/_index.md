---
title: "Clase DynamicFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.DynamicFilter class. Representa el filtro dinámico"
type: docs
url: /es/net/aspose.cells/dynamicfilter/
---
## DynamicFilter class

Representa el filtro dinámico.

```csharp
public class DynamicFilter
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DynamicFilterType](../../aspose.cells/dynamicfilter/dynamicfiltertype/) { get; set; } | Obtiene y establece el tipo de este filtro dinámico. |
| [MaxValue](../../aspose.cells/dynamicfilter/maxvalue/) { get; set; } | Obtiene y establece el valor máximo del filtro dinámico. |
| [Value](../../aspose.cells/dynamicfilter/value/) { get; set; } | Obtiene y establece el valor del filtro dinámico. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un libro de trabajo y una hoja de cálculo (opcional para contexto)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Name = "DemoSheet";

                // Poblar algunos datos numéricos de ejemplo
                worksheet.Cells["A1"].PutValue("Numbers");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);
                worksheet.Cells["A6"].PutValue(50);

                // Definir un rango de autofiltro
                worksheet.AutoFilter.Range = "A1:A6";

                // Aplicar un filtro dinámico (AboveAverage) a la primera columna
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);

                // Recuperar la instancia DynamicFilter creada por el AutoFilter
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // Establezca propiedades adicionales si lo desea
                filter.Value = 25;      // Example custom value
                filter.MaxValue = 45;   // Example max value

                // Mostrar las propiedades establecidas
                Console.WriteLine($"DynamicFilterType: {filter.DynamicFilterType}");
                Console.WriteLine($"Value: {filter.Value}");
                Console.WriteLine($"MaxValue: {filter.MaxValue}");

                // Actualice el filtro para aplicar los cambios
                worksheet.AutoFilter.Refresh();

                // Guardar el libro de trabajo (los datos filtrados se guardarán)
                workbook.Save("DynamicFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DynamicFilter: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


