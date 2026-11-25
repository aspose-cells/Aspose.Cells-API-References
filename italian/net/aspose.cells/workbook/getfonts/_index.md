---
title: "Workbook.GetFonts"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Restituisce tutti i font nel pool di stili"
type: docs
url: /it/net/aspose.cells/workbook/getfonts/
---
## Workbook.GetFonts method

Ottiene tutti i caratteri nel pool di stili.

```csharp
public Font[] GetFonts()
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetFontsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea celle con font diversi
            worksheet.Cells["A1"].PutValue("Sample Text 1");
            worksheet.Cells["A2"].PutValue("Sample Text 2");
            
            // Ottieni e modifica i font
            Font font1 = worksheet.Cells["A1"].GetStyle().Font;
            font1.Name = "Arial";
            font1.Size = 12;
            
            Font font2 = worksheet.Cells["A2"].GetStyle().Font;
            font2.Name = "Times New Roman";
            font2.Size = 14;
            font2.IsBold = true;

            // Ottieni tutti i caratteri utilizzati nella cartella di lavoro
            Font[] fonts = workbook.GetFonts();
            Console.WriteLine("Total fonts in workbook: " + fonts.Length);
            
            // Visualizza le informazioni sui caratteri
            foreach (Font font in fonts)
            {
                Console.WriteLine($"Font: {font.Name}, Size: {font.Size}, Bold: {font.IsBold}");
            }
            
            // Salva e ricarica per dimostrare la persistenza
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, SaveFormat.Xlsx);
                Workbook loadedWorkbook = new Workbook(stream);
                Console.WriteLine("Fonts after save/load: " + loadedWorkbook.GetFonts().Length);
            }
        }
    }
}
```

### Vedi anche

* class [Font](../../font/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


