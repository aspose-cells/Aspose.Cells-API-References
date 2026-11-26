---
title: "ReferredArea.SheetNames"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReferredArea. Nombres de todas las hojas de cálculo a las que esta instancia hace referencia"
type: docs
url: /es/net/aspose.cells/referredarea/sheetnames/
---
## ReferredArea.SheetNames property

Nombres de todas las hojas de cálculo a las que hace referencia esta instancia.

```csharp
public string[] SheetNames { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertySheetNamesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para crear una referencia de fórmula
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Calcular fórmulas para obtener referencias
            workbook.CalculateFormula();

            // Obtener el área referida de la fórmula en A3
            ReferredArea referredArea = worksheet.Cells["A3"].GetPrecedents()[0];

            // Mostrar la propiedad SheetNames
            Console.WriteLine("SheetNames referenced by the formula:");
            if (referredArea.SheetNames != null)
            {
                foreach (string sheetName in referredArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // Agregar otra hoja de cálculo y crear una referencia cruzada entre hojas
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["B1"].PutValue("=Sheet1!A3");

            // Calcular fórmulas nuevamente
            workbook.CalculateFormula();

            // Obtenga el área referida de la fórmula entre hojas
            ReferredArea crossSheetArea = sheet2.Cells["B1"].GetPrecedents()[0];

            // Mostrar SheetNames para referencia entre hojas
            Console.WriteLine("\nSheetNames referenced by cross-sheet formula:");
            if (crossSheetArea.SheetNames != null)
            {
                foreach (string sheetName in crossSheetArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // Guarda el libro de trabajo
            workbook.Save("ReferredAreaSheetNamesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


