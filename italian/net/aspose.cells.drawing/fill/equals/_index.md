---
title: "Fill.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Fill. /"
type: docs
url: /it/net/aspose.cells.drawing/fill/equals/
---
## Fill.Equals method

/

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class FillMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi una forma rettangolare al foglio di lavoro
                Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 0, 0, 100, 150);

                // Ottieni l'oggetto FillFormat dalla forma
                FillFormat fillFormat1 = rectangle.Fill;

                // Crea un'altra forma per ottenere un secondo oggetto FillFormat
                Shape oval = worksheet.Shapes.AddOval(3, 0, 0, 0, 100, 150);
                FillFormat fillFormat2 = oval.Fill;

                // Chiama il metodo Equals per confrontare i due oggetti FillFormat
                bool areEqual = fillFormat1.Equals(fillFormat2);

                // Visualizza il risultato del confronto
                Console.WriteLine($"FillFormat objects are equal: {areEqual}");

                // Mostra anche il confronto con null
                bool isNullEqual = fillFormat1.Equals(null);
                Console.WriteLine($"FillFormat object equals null: {isNullEqual}");

                // Salva la cartella di lavoro
                workbook.Save("FillEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in FillFormat Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Fill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


