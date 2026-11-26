---
title: "ReferredArea.IsEntireRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReferredArea. Indica si esta área contiene todas las columnas o fila completa"
type: docs
url: /es/net/aspose.cells/referredarea/isentirerow/
---
## ReferredArea.IsEntireRow property

Indica si esta área contiene todas las columnas (fila completa).

```csharp
public bool IsEntireRow { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertyIsEntireRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // Crear un rango con nombre que haga referencia a la fila completa 2
            int index1 = workbook.Worksheets.Names.Add("NamedRange1");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$2:$2";

            // Obtener el área referida del rango con nombre
            ReferredArea referredArea = workbook.Worksheets.Names["NamedRange1"].GetReferredAreas(false)[0];

            // Mostrar el valor actual de IsEntireRow
            Console.WriteLine("IsEntireRow value for NamedRange1: " + referredArea.IsEntireRow);

            // Crear otro rango con nombre que haga referencia a un rango específico (no a una fila completa)
            int index2 = workbook.Worksheets.Names.Add("NamedRange2");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1:$B$3";

            // Obtener el área referida del segundo rango con nombre
            ReferredArea referredArea2 = workbook.Worksheets.Names["NamedRange2"].GetReferredAreas(false)[0];

            // Mostrar el valor actual de IsEntireRow para el segundo rango
            Console.WriteLine("IsEntireRow value for NamedRange2: " + referredArea2.IsEntireRow);

            // Demostrar el efecto de IsEntireRow comprobando las dimensiones del rango
            Console.WriteLine("NamedRange1 dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea.StartRow, referredArea.EndRow, referredArea.StartColumn, referredArea.EndColumn);

            Console.WriteLine("NamedRange2 dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea2.StartRow, referredArea2.EndRow, referredArea2.StartColumn, referredArea2.EndColumn);

            // Guarda el libro de trabajo
            workbook.Save("ReferredAreaPropertyIsEntireRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


