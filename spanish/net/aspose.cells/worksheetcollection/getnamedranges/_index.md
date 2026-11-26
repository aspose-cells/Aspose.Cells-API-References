---
title: "WorksheetCollection.GetNamedRanges"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheetcollection/getnamedranges/
---
## WorksheetCollection.GetNamedRanges method

Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo.

```csharp
public Range[] GetNamedRanges()
```

### Valor de retorno

Una matriz de objetos Range. Si la referencia del Nombre definido es externa o tiene múltiples rangos, no se devolverá ningún objeto Range para este Nombre.

Devuelve null si el rango con nombre no existe.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodGetNamedRangesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear algunos rangos con nombre para demostración
            worksheet.Cells.CreateRange("A1:B2").Name = "SalesData";
            worksheet.Cells.CreateRange("C3:D4").Name = "Expenses";

            try
            {
                // Llamar al método GetNamedRanges para recuperar todos los rangos con nombre
                Aspose.Cells.Range[] namedRanges = workbook.Worksheets.GetNamedRanges();

                // Mostrar información sobre los rangos con nombre
                Console.WriteLine("Found {0} named ranges:", namedRanges.Length);
                foreach (Aspose.Cells.Range range in namedRanges)
                {
                    Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
                }

                // Guarda el libro de trabajo
                workbook.Save("GetNamedRangesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNamedRanges: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


