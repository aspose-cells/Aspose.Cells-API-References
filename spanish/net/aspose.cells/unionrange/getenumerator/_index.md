---
title: "UnionRange.GetEnumerator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método UnionRange. Obtiene el enumerador para las celdas en este rango"
type: docs
url: /es/net/aspose.cells/unionrange/getenumerator/
---
## UnionRange.GetEnumerator method

Obtiene el enumerador de celdas en este Rango.

```csharp
public IEnumerator GetEnumerator()
```

### Valor de retorno

El enumerador de celdas

### Observaciones

Al recorrer los elementos mediante el Enumerator devuelto, la colección de celdas no debe modificarse (por ejemplo, operaciones que provoquen la creación de nuevas Cell/Row o la eliminación de Cell/Row existentes). De lo contrario, el enumerador podría no ser capaz de recorrer todas las celdas correctamente (algunos elementos podrían recorrerse repetidamente o omitirse).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class UnionRangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea el primer rango (A1:B2) y llénalo con datos
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1", "B2");
            range1[0, 0].PutValue("R1C1");
            range1[0, 1].PutValue("R1C2");
            range1[1, 0].PutValue("R2C1");
            range1[1, 1].PutValue("R2C2");

            // Crea el segundo rango (C1:D2) y llénalo con datos
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C1", "D2");
            range2[0, 0].PutValue("R1C3");
            range2[0, 1].PutValue("R1C4");
            range2[1, 0].PutValue("R2C3");
            range2[1, 1].PutValue("R2C4");

            try
            {
                // Construye un UnionRange a partir del primer rango
                UnionRange unionRange = worksheet.Cells
                    .CreateRange("A1:B2")
                    .UnionRanges(new Aspose.Cells.Range[] { range1 });

                // Agrega el segundo rango a la unión
                unionRange = unionRange.Union("C1:D2");

                // Obtén el enumerador e itera a través de todas las celdas en la unión
                IEnumerator enumerator = unionRange.GetEnumerator();
                Console.WriteLine("Enumerating cells in the UnionRange:");
                while (enumerator.MoveNext())
                {
                    Cell cell = enumerator.Current as Cell;
                    if (cell != null)
                    {
                        Console.WriteLine($"{cell.Name}: {cell.Value}");
                    }
                }

                // Guarda el libro de trabajo (opcional, solo para mostrar que los datos persisten)
                workbook.Save("UnionRangeGetEnumeratorDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetEnumerator: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


