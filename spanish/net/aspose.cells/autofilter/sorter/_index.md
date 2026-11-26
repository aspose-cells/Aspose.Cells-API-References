---
title: "AutoFilter.Sorter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoFilter. Obtiene el ordenamiento de datos"
type: docs
url: /es/net/aspose.cells/autofilter/sorter/
---
## AutoFilter.Sorter property

Obtiene el ordenador de datos.

```csharp
public DataSorter Sorter { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertySorterDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // Crear rango de autofiltro
            worksheet.AutoFilter.Range = "A1:B4";

            // Obtener el filtro automático
            AutoFilter filter = worksheet.AutoFilter;

            // Aplicar filtro
            filter.Filter(1, "10");

            // Ordenar usando la propiedad Sorter
            filter.Sorter.Sort();

            // Guarda el libro de trabajo
            workbook.Save("AutoFilterPropertySorterDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataSorter](../../datasorter/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


