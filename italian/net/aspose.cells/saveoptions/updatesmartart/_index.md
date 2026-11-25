---
title: "SaveOptions.UpdateSmartArt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SaveOptions. Indica se aggiornare l'impostazione di SmartArt. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/saveoptions/updatesmartart/
---
## SaveOptions.UpdateSmartArt property

Indica se aggiornare l'impostazione SmartArt. Il valore predefinito è false.

```csharp
public bool UpdateSmartArt { get; set; }
```

### Osservazioni

Ha effetto solo dopo aver chiamato il metodo Shape.GetResultOfSmartArt() e quando le forme memorizzate nella cache esistono nel file modello.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyUpdateSmartArtDemo
    {
        public static void Run()
        {
            // Carica la cartella di lavoro di origine
            Workbook workbook = new Workbook("example.xlsx");

            // Modifica forme e SmartArt
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                foreach (Shape shape in worksheet.Shapes)
                {
                    shape.AlternativeText = "ReplacedAlternativeText";
                    
                    if (shape.IsSmartArt)
                    {
                        foreach (Shape smartArtShape in shape.GetResultOfSmartArt().GetGroupedShapes())
                        {
                            smartArtShape.Text = "ReplacedText";
                        }
                    }
                }
            }

            // Salva con UpdateSmartArt abilitato
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.UpdateSmartArt = true;
            workbook.Save("output.xlsx", saveOptions);

            // Verifica le modifiche
            Workbook savedWorkbook = new Workbook("output.xlsx");
            foreach (Worksheet worksheet in savedWorkbook.Worksheets)
            {
                foreach (Shape shape in worksheet.Shapes)
                {
                    Console.WriteLine($"Shape Alt Text: {shape.AlternativeText}");
                    
                    if (shape.IsSmartArt)
                    {
                        foreach (Shape smartArtShape in shape.GetResultOfSmartArt().GetGroupedShapes())
                        {
                            Console.WriteLine($"SmartArt Text: {smartArtShape.Text}");
                        }
                    }
                }
            }
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


