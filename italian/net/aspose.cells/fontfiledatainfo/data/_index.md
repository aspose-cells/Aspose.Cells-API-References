---
title: "FontFileDataInfo.Data"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FontFileDataInfo. Ottiene i dati binari del file di carattere"
type: docs
url: /it/net/aspose.cells/fontfiledatainfo/data/
---
## FontFileDataInfo.Data property

Ottiene i dati binari del file di carattere.

```csharp
public byte[] Data { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Carica un file di carattere (sostituisci con il percorso reale del file di carattere)
            string fontFilePath = "samplefont.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // Crea un'istanza di FontConfigs e aggiungi il carattere
            FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);
            
            // In un uso reale, FontFileDataInfo verrebbe ottenuto dalla libreria
            // Per scopi dimostrativi, mostreremo semplicemente come lo useresti se ne avessi uno
            FontFileDataInfo fontInfo = null; // Normally obtained from library APIs
            
            // Visualizza le informazioni sui dati del carattere (se disponibili)
            Console.WriteLine("Font data length: " + (fontInfo?.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
            }

            // In un uso reale, la proprietà Data verrebbe usata per accedere ai dati binari del carattere
            // Ad esempio, potresti salvarlo in un file:
            if (fontInfo?.Data != null && fontInfo.Data.Length > 0)
            {
                File.WriteAllBytes("extracted_font.ttf", fontInfo.Data);
                Console.WriteLine("Font data extracted to file.");
            }

            // Salva la cartella di lavoro (il carattere influirebbe sul rendering se usato nelle celle)
            workbook.Save("FontDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


