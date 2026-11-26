---
title: "DynamicFilter.MaxValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DynamicFilter. Obtiene y establece el valor máximo del filtro dinámico"
type: docs
url: /es/net/aspose.cells/dynamicfilter/maxvalue/
---
## DynamicFilter.MaxValue property

Obtiene y establece el valor máximo del filtro dinámico.

```csharp
public object MaxValue { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyMaxValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos numéricos de ejemplo
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);

            // Cree filtro automático
            worksheet.AutoFilter.Range = "A1:A6";
            
            // Aplicar filtro dinámico con criterios de rango
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // Mostrar el MaxValue actual
            Console.WriteLine("Current MaxValue: " + filter.MaxValue);

            // Dado que DynamicFilterType.Between no existe, utilizaremos un enfoque diferente
            // Por ejemplo, podemos usar un filtro personalizado en su lugar
            worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterOrEqual, 20);
            worksheet.AutoFilter.Custom(0, FilterOperatorType.LessOrEqual, 40);

            // Aplicar el filtro
            worksheet.AutoFilter.Refresh();

            // Guardar el resultado
            workbook.Save("DynamicFilterMaxValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


