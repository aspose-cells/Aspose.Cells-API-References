---
title: "Font.Color"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Font. Ottiene o imposta il Color del font"
type: docs
url: /it/net/aspose.cells/font/color/
---
## Font.Color property

Ottiene o imposta il colore del font.

```csharp
public Color Color { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FontPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta HTML con diversi colori e stili di carattere
            Cell cell = worksheet.Cells["A1"];
            cell.HtmlString = "<font color='Red'>Red Text</font> <font color='#0000FF'>Blue Text</font><font style='color:#00FF00;text-decoration: underline;'>Green Underlined</font>";
            
            // Ottieni la formattazione del testo ricco
            FontSetting[] richText = cell.GetCharacters();
            
            // Verifica e dimostra le proprietà del colore
            Console.WriteLine("First segment color: " + richText[0].Font.Color);
            Console.WriteLine("Second segment color: " + richText[1].Font.Color);
            Console.WriteLine("Third segment underline: " + richText[2].Font.Underline);
            
            // Salva la cartella di lavoro
            workbook.Save("FontColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


