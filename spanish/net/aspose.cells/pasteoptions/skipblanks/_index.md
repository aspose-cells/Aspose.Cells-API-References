---
title: "PasteOptions.SkipBlanks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PasteOptions. Indica si se omiten celdas en blanco"
type: docs
url: /es/net/aspose.cells/pasteoptions/skipblanks/
---
## PasteOptions.SkipBlanks property

Indica si se omiten celdas en blanco.

```csharp
public bool SkipBlanks { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertySkipBlanksDemo
    {
        public static void Run()
        {
            // Cree un libro de trabajo de origen con datos de muestra
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Rellenar el rango de origen con algunos valores y celdas en blanco
            sourceSheet.Cells["A1"].PutValue("Value 1");
            sourceSheet.Cells["A2"].PutValue(""); // Blank cell
            sourceSheet.Cells["A3"].PutValue("Value 3");
            sourceSheet.Cells["A4"].PutValue(""); // Blank cell
            
            // Cree un libro de trabajo de destino
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Rellenar el rango de destino con valores existentes
            destSheet.Cells["A1"].PutValue("Existing 1");
            destSheet.Cells["A2"].PutValue("Existing 2");
            destSheet.Cells["A3"].PutValue("Existing 3");
            destSheet.Cells["A4"].PutValue("Existing 4");
            
            // Obtener rangos con nombres de tipo totalmente calificados
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.CreateRange("A1:A4");
            Aspose.Cells.Range destRange = destSheet.Cells.CreateRange("A1:A4");
            
            // Copiar con SkipBlanks = true (predeterminado)
            destRange.Copy(sourceRange, new PasteOptions { SkipBlanks = true });
            
            Console.WriteLine("Results with SkipBlanks=true:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {destSheet.Cells[i, 0].StringValue}");
            }
            
            // Restablecer los valores de destino
            destSheet.Cells["A1"].PutValue("Existing 1");
            destSheet.Cells["A2"].PutValue("Existing 2");
            destSheet.Cells["A3"].PutValue("Existing 3");
            destSheet.Cells["A4"].PutValue("Existing 4");
            
            // Copiar con SkipBlanks = false
            destRange.Copy(sourceRange, new PasteOptions { SkipBlanks = false });
            
            Console.WriteLine("\nResults with SkipBlanks=false:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {destSheet.Cells[i, 0].StringValue}");
            }
        }
    }
}
```

### Ver también

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


