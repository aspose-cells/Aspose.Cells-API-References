---
title: "ReferredArea.IsEntireColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReferredArea. Indica si esta área contiene todas las filas o la columna completa"
type: docs
url: /es/net/aspose.cells/referredarea/isentirecolumn/
---
## ReferredArea.IsEntireColumn property

Indica si este área contiene todas las filas (columna completa).

```csharp
public bool IsEntireColumn { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertyIsEntireColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);

            // Crear un rango nombrado que haga referencia a la columna completa B
            int index = workbook.Worksheets.Names.Add("PriceColumn");
            workbook.Worksheets.Names[index].RefersTo = "=Sheet1!$B:$B";

            // Obtener el área referida del rango con nombre
            ReferredArea referredArea = workbook.Worksheets.Names["PriceColumn"].GetReferredAreas(false)[0];

            // Mostrar el valor de la propiedad IsEntireColumn
            Console.WriteLine("IsEntireColumn value for PriceColumn: " + referredArea.IsEntireColumn);

            // Crear otro rango nombrado que haga referencia a un rango específico (no a la columna completa)
            int index2 = workbook.Worksheets.Names.Add("ProductRange");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1:$B$3";

            // Obtener el área referida del segundo rango con nombre
            ReferredArea referredArea2 = workbook.Worksheets.Names["ProductRange"].GetReferredAreas(false)[0];

            // Mostrar el valor de la propiedad IsEntireColumn para el segundo rango
            Console.WriteLine("IsEntireColumn value for ProductRange: " + referredArea2.IsEntireColumn);

            // Demostrar el efecto de IsEntireColumn comprobando las dimensiones del rango
            Console.WriteLine("PriceColumn dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea.StartRow, referredArea.EndRow, referredArea.StartColumn, referredArea.EndColumn);

            Console.WriteLine("ProductRange dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea2.StartRow, referredArea2.EndRow, referredArea2.StartColumn, referredArea2.EndColumn);

            // Guarda el libro de trabajo
            workbook.Save("ReferredAreaPropertyIsEntireColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


