---
title: "FontFileDataInfo.FormatType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FontFileDataInfo. Ottiene il tipo di formato del font del file"
type: docs
url: /it/net/aspose.cells/fontfiledatainfo/formattype/
---
## FontFileDataInfo.FormatType property

Ottiene il tipo di formato del file di carattere.

```csharp
public FontFileFormatType FormatType { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyFormatTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi del testo per dimostrare l'uso del carattere
            worksheet.Cells["A1"].PutValue("Sample Text with Font");

            try
            {
                // Carica un file di carattere di esempio (sostituisci con il percorso reale del file di carattere)
                string fontFilePath = "arial.ttf";
                if (File.Exists(fontFilePath))
                {
                    // Registra la cartella dei caratteri
                    FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);

                    // In uno scenario reale, FontFileDataInfo verrebbe ottenuto dalla libreria
                    // Per dimostrazione, simuleremo l'ottenimento delle informazioni sul carattere
                    // Nota: l'API reale potrebbe fornire questo tramite FontConfigs o simili
                    FontFileDataInfo fontInfo = GetFontFileDataInfo(fontFilePath);

                    if (fontInfo != null)
                    {
                        // Visualizza il valore della proprietà FormatType
                        Console.WriteLine("Font Format Type: " + fontInfo.FormatType);

                        // Mostra il valore enum come stringa
                        Console.WriteLine("Format Type Description: " +
                            Enum.GetName(typeof(FontFileFormatType), fontInfo.FormatType));

                        // Applica il carattere a una cella (concettuale - l'implementazione reale può variare)
                        Style style = worksheet.Cells["A1"].GetStyle();
                        style.Font.Name = "Arial";
                        worksheet.Cells["A1"].SetStyle(style);
                    }
                    else
                    {
                        Console.WriteLine("Font information could not be retrieved");
                    }
                }
                else
                {
                    Console.WriteLine("Font file not found at: " + fontFilePath);
                }

                // Salva la cartella di lavoro
                workbook.Save("FormatTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Metodo di supporto per simulare l'ottenimento di FontFileDataInfo
        // In un uso reale, questo sarebbe fornito dall'API Aspose.Cells
        private static FontFileDataInfo GetFontFileDataInfo(string fontPath)
        {
            try
            {
                byte[] fontData = File.ReadAllBytes(fontPath);
                string extension = Path.GetExtension(fontPath).ToLower();

                // Crea un mock di FontFileDataInfo (in realtà, questo verrebbe dall'API)
                // Poiché non possiamo istanziarlo direttamente, simuleremo il comportamento
                FontFileFormatType formatType = FontFileFormatType.Unknown;

                if (extension == ".ttf")
                    formatType = FontFileFormatType.Ttf;
                else if (extension == ".otf")
                    formatType = FontFileFormatType.Otf;
                else if (extension == ".ttc")
                    formatType = FontFileFormatType.Ttc;

                // In un'implementazione reale, questo verrebbe restituito dall'API
                // Per questa demo, restituiremo semplicemente null poiché non possiamo creare l'oggetto
                Console.WriteLine($"Detected font format: {formatType}");
                return null;
            }
            catch
            {
                return null;
            }
        }
    }
}
```

### Vedi anche

* enum [FontFileFormatType](../../fontfileformattype/)
* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


