---
title: "DeleteBlankOptions.DrawingsAsBlank"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DeleteBlankOptions. Indica se gli oggetti correlati ai disegni, come immagini, forme, grafici... saranno considerati vuoti. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/deleteblankoptions/drawingsasblank/
---
## DeleteBlankOptions.DrawingsAsBlank property

Indica se gli oggetti correlati al disegno, come immagine, forma, grafico... saranno considerati vuoti. Il valore predefinito è true.

```csharp
public bool DrawingsAsBlank { get; set; }
```

### Osservazioni

Impostando questa proprietà su false, tutte le righe/colonne coperte da oggetti di disegno non saranno considerate vuote e non verranno eliminate.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyDrawingsAsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data");
            worksheet.Cells["B1"].PutValue("");
            worksheet.Cells["B2"].PutValue("");

            // Aggiungi un oggetto di disegno per testare il comportamento di DrawingsAsBlank
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);

            // Elimina le colonne vuote con DrawingsAsBlank = false (preserva i disegni)
            worksheet.Cells.DeleteBlankColumns(new DeleteBlankOptions { DrawingsAsBlank = false });

            Console.WriteLine("Drawing preserved count: " + worksheet.Shapes.Count);
        }
    }
}
```

### Vedi anche

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


