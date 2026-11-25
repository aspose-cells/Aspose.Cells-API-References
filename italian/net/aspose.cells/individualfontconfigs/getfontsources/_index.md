---
title: "IndividualFontConfigs.GetFontSources"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo IndividualFontConfigs. Ottiene una copia dell'array che contiene l'elenco delle sorgenti"
type: docs
url: /it/net/aspose.cells/individualfontconfigs/getfontsources/
---
## IndividualFontConfigs.GetFontSources method

Ottiene una copia dell'array che contiene l'elenco delle fonti.

```csharp
public FontSourceBase[] GetFontSources()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSourcesDemo
    {
        public static void Run()
        {
            // Crea configurazioni di font individuali
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Imposta alcune sorgenti di font (cartelle contenenti font)
            string fontFolder1 = @"C:\Windows\Fonts";
            string fontFolder2 = @"D:\CustomFonts";
            fontConfigs.SetFontFolder(fontFolder1, false);
            fontConfigs.SetFontFolder(fontFolder2, true);

            try
            {
                // Ottieni le font source attuali
                FontSourceBase[] fontSources = fontConfigs.GetFontSources();

                Console.WriteLine("Current font sources:");
                foreach (var source in fontSources)
                {
                    if (source is FolderFontSource folderSource)
                    {
                        Console.WriteLine($"- Folder: {folderSource.FolderPath} (Recursive: {folderSource.ScanSubFolders})");
                    }
                }

                // Crea una cartella di lavoro per dimostrare l'effetto
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                // Usa le configurazioni dei font quando crei stili o lavori con i font
                // (La cartella di lavoro non ha una proprietà FontConfigs, quindi rimuoviamo quella riga)
                Worksheet worksheet = workbook.Worksheets[0];

                // Usa un font personalizzato che potrebbe trovarsi in una delle cartelle
                Style style = workbook.CreateStyle();
                style.Font.Name = "SomeCustomFont";
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text with custom font");

                Console.WriteLine("Workbook created with custom font configurations.");
                workbook.Save("MethodGetFontSourcesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontSources method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [FontSourceBase](../../fontsourcebase/)
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


