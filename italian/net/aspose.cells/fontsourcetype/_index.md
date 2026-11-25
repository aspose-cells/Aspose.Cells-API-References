---
title: "Enum FontSourceType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.FontSourceType. Specifica il tipo di una sorgente di font"
type: docs
url: /it/net/aspose.cells/fontsourcetype/
---
## FontSourceType enumeration

Specifica il tipo di origine del carattere.

```csharp
public enum FontSourceType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| FontFile | `0` | rappresenta un singolo file di font. |
| FontsFolder | `1` | Rappresenta una cartella con file di font. |
| MemoryFont | `2` | Rappresenta un singolo font in memoria. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontSourceTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dimostra i valori dell'enumerazione FontSourceType
            Console.WriteLine("FontSourceType values:");
            Console.WriteLine($"FontFile: {FontSourceType.FontFile}");
            Console.WriteLine($"FontsFolder: {FontSourceType.FontsFolder}");
            Console.WriteLine($"MemoryFont: {FontSourceType.MemoryFont}");

            // Crea impostazioni dei font e utilizza FontSourceType
            FontConfigs.SetFontFolder(@"C:\MyFonts\", false);
            FontConfigs.SetFontSources(new FontSourceBase[]
            {
                new FolderFontSource(@"C:\MyFonts\", false),
                new FileFontSource(@"C:\MyFonts\arial.ttf"),
                new MemoryFontSource(new byte[0])
            });

            // Applica il font a una cella
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with Arial font");

            // Salva il risultato
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


