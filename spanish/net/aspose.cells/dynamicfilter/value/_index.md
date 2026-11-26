---
title: "DynamicFilter.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DynamicFilter. Obtiene y establece el valor del filtro dinámico"
type: docs
url: /es/net/aspose.cells/dynamicfilter/value/
---
## DynamicFilter.Value property

Obtiene y establece el valor del filtro dinámico.

```csharp
public object Value { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            // Cree filtro automático
            worksheet.AutoFilter.Range = "A1:A5";
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // Muestre el valor actual del filtro
            Console.WriteLine("Current DynamicFilter Value: " + filter.Value);

            // Cambie el valor del filtro para mostrar fechas de abril
            filter.Value = new DateTime(2023, 4, 1);
            filter.DynamicFilterType = DynamicFilterType.April;

            // Aplicar el filtro
            worksheet.AutoFilter.Refresh();

            // Guardar el resultado
            workbook.Save("DynamicFilterValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


