---
title: "IndividualFontConfigs.SetFontFolders"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo IndividualFontConfigs. Imposta le cartelle dei font"
type: docs
url: /it/net/aspose.cells/individualfontconfigs/setfontfolders/
---
## IndividualFontConfigs.SetFontFolders method

Imposta le cartelle dei caratteri

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
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

    public class IndividualFontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Prepara l'array delle cartelle dei font
            string[] fontFolders = new string[] { @"C:\Windows\Fonts", @"D:\CustomFonts" };
            bool recursiveSearch = true;

            try
            {
                // Chiama il metodo SetFontFolders con parametri String[] e Boolean
                fontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // Dimostra l'effetto usando un font personalizzato
                worksheet.Cells["A1"].PutValue("Text with custom font");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Assuming this font exists in one of the folders
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("SetFontFolders method executed successfully with parameters (String[], Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontFolders method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("SetFontFoldersDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


