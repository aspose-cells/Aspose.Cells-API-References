---
title: "DynamicFilter.DynamicFilterType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DynamicFilter. Obtiene y establece el tipo de este filtro dinámico"
type: docs
url: /es/net/aspose.cells/dynamicfilter/dynamicfiltertype/
---
## DynamicFilter.DynamicFilterType property

Obtiene y establece el tipo de este filtro dinámico.

```csharp
public DynamicFilterType DynamicFilterType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyDynamicFilterTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra con fechas
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            try
            {
                // Cree filtro automático
                worksheet.AutoFilter.Range = "A1:A5";

                // Aplicar filtro dinámico para fechas de marzo
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

                // Obtener la instancia de DynamicFilter
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // Mostrar el valor actual de DynamicFilterType
                Console.WriteLine("Current DynamicFilterType: " + filter.DynamicFilterType);

                // Cambiar el tipo de filtro para mostrar fechas de abril
                filter.DynamicFilterType = DynamicFilterType.April;

                // Mostrar el valor actualizado de DynamicFilterType
                Console.WriteLine("Updated DynamicFilterType: " + filter.DynamicFilterType);

                // Aplicar el filtro
                worksheet.AutoFilter.Refresh();

                // Guardar el resultado
                workbook.Save("DynamicFilterTypeDemo.xlsx");
                Console.WriteLine("DynamicFilterType has been demonstrated successfully.");
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

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


