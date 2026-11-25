---
title: "FontSetting.Length"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FontSetting. Ottiene la lunghezza dei caratteri"
type: docs
url: /it/net/aspose.cells/fontsetting/length/
---
## FontSetting.Length property

Ottiene la lunghezza dei caratteri.

```csharp
public int Length { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingPropertyLengthDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e accedi al suo primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi del testo alla cella A1
            worksheet.Cells["A1"].PutValue("Hello World");

            // Crea le impostazioni del carattere per il testo nella cella A1
            FontSetting fontSetting = worksheet.Cells["A1"].Characters(0, 5);
            
            // Dimostra l'uso della proprietà Length
            Console.WriteLine("Original Length: " + fontSetting.Length);
            
            // Modifica la lunghezza dell'impostazione del carattere
            fontSetting = worksheet.Cells["A1"].Characters(0, 11);
            Console.WriteLine("Modified Length: " + fontSetting.Length);
            
            // Applica la formattazione all'impostazione del carattere
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // Salva la cartella di lavoro
            workbook.Save("FontSettingLengthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


