---
title: "Enum FormatSetType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.FormatSetType enum. Tipo di set di formato di riempimento"
type: docs
url: /it/net/aspose.cells.drawing/formatsettype/
---
## FormatSetType enumeration

Tipo di set di formato di riempimento.

```csharp
public enum FormatSetType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessun formato di riempimento. |
| IsGradientSet | `1` | Formato di riempimento a gradiente. |
| IsTextureSet | `2` | Formato di riempimento a trama. |
| IsPatternSet | `3` | Formato di riempimento a motivo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassFormatSetTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi una forma per dimostrare il formato di riempimento
                Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
                FillFormat fillFormat = shape.Fill;

                // Visualizza il tipo di riempimento iniziale
                Console.WriteLine("Initial fill type: " + fillFormat.Type);

                // Dimostra i valori dell'enum FormatSetType
                Console.WriteLine("FormatSetType.None: " + (int)FormatSetType.None);
                Console.WriteLine("FormatSetType.IsGradientSet: " + (int)FormatSetType.IsGradientSet);
                Console.WriteLine("FormatSetType.IsTextureSet: " + (int)FormatSetType.IsTextureSet);
                Console.WriteLine("FormatSetType.IsPatternSet: " + (int)FormatSetType.IsPatternSet);

                // Applica diversi tipi di riempimento usando FormatSetType
                fillFormat.Type = (FillType)FormatSetType.IsGradientSet;
                Console.WriteLine("After setting gradient: " + fillFormat.Type);

                fillFormat.Type = (FillType)FormatSetType.IsPatternSet;
                Console.WriteLine("After setting pattern: " + fillFormat.Type);

                // Salva la cartella di lavoro
                workbook.Save("FormatSetTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with FormatSetType: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


