---
title: "FontConfigs.GetFontFileDataInfo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontConfigs. Ottieni le informazioni sui dati del file del font"
type: docs
url: /it/net/aspose.cells/fontconfigs/getfontfiledatainfo/
---
## FontConfigs.GetFontFileDataInfo method

Ottieni le informazioni sui dati del file del carattere.

```csharp
public static FontFileDataInfo GetFontFileDataInfo(string fontName, bool isBold, bool isItalic, 
    bool isExactStyle)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontName | String | nome del font |
| isBold | Booleano | lo stile del font è grassetto o meno |
| isItalic | Booleano | lo stile del font è corsivo o meno |
| isExactStyle | Booleano | se corrispondere esattamente allo stile grassetto/corsivo fornito |

### Valore di ritorno

Informazioni sui dati del file del font.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodGetFontFileDataInfoWithStringBooleanBooleanBooleanDemo
    {
        public static void Run()
        {
            try
            {
                // Chiama GetFontFileDataInfo con parametri specifici (modificato a chiamata statica)
                FontFileDataInfo fontInfo = FontConfigs.GetFontFileDataInfo("Arial", true, false, false);

                // Visualizza le informazioni sui dati del file di carattere
                if (fontInfo != null)
                {
                    Console.WriteLine($"Font format type: {fontInfo.FormatType}");
                    Console.WriteLine($"Font data length: {fontInfo.Data?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Font information not available");
                }

                // Dimostra l'effetto su una cartella di lavoro
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Imposta lo stile con il carattere che abbiamo verificato
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.IsBold = true;
                style.Font.IsItalic = false;
                
                // Applica lo stile a una cella
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text with Arial Bold");

                // Salva la cartella di lavoro
                workbook.Save("FontConfigsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontFileDataInfo method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [FontFileDataInfo](../../fontfiledatainfo/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


