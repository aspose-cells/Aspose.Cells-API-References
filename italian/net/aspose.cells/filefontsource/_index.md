---
title: "Classe FileFontSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.FileFontSource. Rappresenta il singolo file di font TrueType memorizzato nel file system"
type: docs
url: /it/net/aspose.cells/filefontsource/
---
## FileFontSource class

Rappresenta il singolo file di font TrueType memorizzato nel file system.

```csharp
public class FileFontSource : FontSourceBase
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [FileFontSource](filefontsource/)(string) | Ctor. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FilePath](../../aspose.cells/filefontsource/filepath/) { get; } | Percorso del file di font. |
| override [Type](../../aspose.cells/filefontsource/type/) { get; } | Restituisce il tipo della fonte del font. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFontSourceDemo
    {
        public static void FileFontSourceExample()
        {
            // Specifica il percorso del file di font TrueType
            string fontFilePath = "C:\\Fonts\\CustomFont.ttf";

            // Crea un'istanza di FileFontSource
            FileFontSource fontSource = new FileFontSource(fontFilePath);

            // Visualizza il tipo di origine del font e il percorso del file
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            Console.WriteLine("Font File Path: " + fontSource.FilePath);

            // Crea un oggetto Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Imposta un valore di cella
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Hello, Aspose!");

            // Applica il font personalizzato alla cella
            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont"; // Use the name of the font
            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("FileFontSourceExample.xlsx");
            workbook.Save("FileFontSourceExample.pdf");
        }
    }
}
```

### Vedi anche

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


