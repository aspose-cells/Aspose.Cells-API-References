---
title: "IndividualFontConfigs.SetFontFolder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo IndividualFontConfigs. Imposta la cartella dei font"
type: docs
url: /it/net/aspose.cells/individualfontconfigs/setfontfolder/
---
## IndividualFontConfigs.SetFontFolder method

Imposta la cartella dei caratteri

```csharp
public void SetFontFolder(string fontFolder, bool recursive)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontFolder | String | La cartella che contiene i font TrueType. |
| ricorsivo | Booleano | Determina se scansionare o meno le sottocartelle. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // Crea un'istanza di IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();
            
            // Specifica il percorso della cartella dei font e se cercare ricorsivamente
            string fontFolderPath = @"C:\Windows\Fonts";
            bool recursiveSearch = true;

            try
            {
                // Chiama SetFontFolder con i parametri specificati
                fontConfigs.SetFontFolder(fontFolderPath, recursiveSearch);
                
                Console.WriteLine($"Successfully set font folder to: {fontFolderPath}");
                Console.WriteLine($"Recursive search enabled: {recursiveSearch}");

                // Crea una cartella di lavoro per dimostrare l'uso dei font
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Imposta uno stile che potrebbe utilizzare i font dalla cartella specificata
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial"; // Assuming Arial exists in the font folder
                style.Font.Size = 12;
                
                worksheet.Cells["A1"].Value = "Text with font from specified folder";
                worksheet.Cells["A1"].SetStyle(style);
                
                // Salva la cartella di lavoro
                workbook.Save("FontConfigDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font folder: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


