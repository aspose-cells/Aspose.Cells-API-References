---
title: "FontConfigs.SetFontFolders"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontConfigs. Imposta la cartella dei font"
type: docs
url: /it/net/aspose.cells/fontconfigs/setfontfolders/
---
## FontConfigs.SetFontFolders method

Imposta la cartella dei caratteri

```csharp
public static void SetFontFolders(string[] fontFolders, bool recursive)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontFolders | String[] | Le cartelle che contengono i font TrueType. |
| ricorsivo | Booleano | Determina se scansionare o meno le sottocartelle. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta del testo che utilizzerà i font personalizzati
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // Prepara le cartelle dei font (sostituisci con i percorsi effettivi sul tuo sistema)
            string[] fontFolders = new string[] 
            {
                @"C:\Windows\Fonts",
                @"D:\CustomFonts"
            };
            bool recursiveSearch = true;

            try
            {
                // Chiama il metodo SetFontFolders con parametri String[] e Boolean
                FontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // Applica un font che potrebbe trovarsi in una di queste cartelle
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Replace with actual font name
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("Font folders set successfully. Workbook may use fonts from these locations.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font folders: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("FontConfigsSetFontFoldersDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


