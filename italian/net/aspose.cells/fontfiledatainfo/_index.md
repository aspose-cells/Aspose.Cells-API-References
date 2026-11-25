---
title: "Classe FontFileDataInfo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.FontFileDataInfo. Rappresenta le informazioni dei dati del file di carattere"
type: docs
url: /it/net/aspose.cells/fontfiledatainfo/
---
## FontFileDataInfo class

Rappresenta le informazioni dei dati del file di font.

```csharp
public class FontFileDataInfo
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Data](../../aspose.cells/fontfiledatainfo/data/) { get; } | Ottiene i dati binari del file di carattere. |
| [FormatType](../../aspose.cells/fontfiledatainfo/formattype/) { get; } | Ottiene il tipo di formato del file di carattere. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassFontFileDataInfoDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Esempio: Caricamento dei dati del file di carattere
            string fontFilePath = "arial.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // Nota: FontFileDataInfo non può essere istanziato direttamente poiché non ha un costruttore pubblico
            // e le sue proprietà sono di sola lettura. In uno scenario reale, otterresti un'istanza
            // da un altro metodo API (come FontConfigs.GetFontFileDataInfo())
            FontFileDataInfo fontInfo = null; // Would be populated by API call in real scenario

            // Dimostrare come verrebbero usate le proprietà se avessimo un'istanza
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
                Console.WriteLine("Font data length: " + (fontInfo.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            }

            // Dimostrare l'integrazione con Workbook
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // Salva la cartella di lavoro
            workbook.Save("FontFileDataInfoDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


