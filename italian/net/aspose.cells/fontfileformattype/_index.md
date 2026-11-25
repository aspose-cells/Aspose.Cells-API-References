---
title: "Enum FontFileFormatType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.FontFileFormatType enum. Rappresenta il tipo di formato del carattere"
type: docs
url: /it/net/aspose.cells/fontfileformattype/
---
## FontFileFormatType enumeration

Rappresenta il tipo di formato del carattere.

```csharp
public enum FontFileFormatType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Unknown | `0` | Tipo di formato del carattere sconosciuto. |
| Ttf | `1` | Tipo di formato del carattere TTF. |
| Otf | `2` | Tipo di formato del carattere OTF. |
| Ttc | `3` | Tipo di formato del carattere TTC. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontFileFormatTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi a una cella e imposta il suo stile
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Font Format Type Demo");
            Style style = cell.GetStyle();

            // Dimostra l'uso di FontFileFormatType
            FontFileFormatType fontFormat = FontFileFormatType.Ttf;
            Console.WriteLine("Selected font format: " + fontFormat.ToString());

            // Applica le impostazioni del carattere
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Verifica la compatibilità del formato del carattere
            if (fontFormat == FontFileFormatType.Ttf)
            {
                Console.WriteLine("Using TrueType font format");
            }

            // Salva la cartella di lavoro
            workbook.Save("FontFileFormatTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


