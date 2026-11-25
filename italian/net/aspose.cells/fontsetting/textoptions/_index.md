---
title: "FontSetting.TextOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FontSetting. Restituisce le opzioni di testo"
type: docs
url: /it/net/aspose.cells/fontsetting/textoptions/
---
## FontSetting.TextOptions property

Restituisce le opzioni di testo.

```csharp
public TextOptions TextOptions { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingPropertyTextOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea testo di esempio con diverse sezioni di formattazione
            string part1 = "This is normal text. ";
            string part2 = "This is bold and italic text. ";
            string part3 = "This is normal again. ";
            string part4 = "This is bold text.";
            
            // Combina tutte le parti in una singola cella
            Cell cell = worksheet.Cells["A1"];
            cell.Value = part1 + part2 + part3 + part4;
            
            // Applica la formattazione a parti specifiche del testo
            int startPos1 = part1.Length;
            int length1 = part2.Length;
            cell.Characters(startPos1, length1).TextOptions.IsBold = true;
            cell.Characters(startPos1, length1).TextOptions.IsItalic = true;
            
            int startPos2 = part1.Length + part2.Length + part3.Length;
            int length2 = part4.Length;
            cell.Characters(startPos2, length2).TextOptions.IsBold = true;
            
            // Salva la cartella di lavoro
            workbook.Save("TextOptionsDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("TextOptions demo completed. File saved.");
        }
    }
}
```

### Vedi anche

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


