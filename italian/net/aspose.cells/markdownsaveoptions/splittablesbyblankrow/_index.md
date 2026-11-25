---
title: "MarkdownSaveOptions.SplitTablesByBlankRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MarkdownSaveOptions. Indica se le righe vuote nel foglio di lavoro devono essere trattate come separatori di tabella durante l'esportazione in Markdown. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/markdownsaveoptions/splittablesbyblankrow/
---
## MarkdownSaveOptions.SplitTablesByBlankRow property

Indica se le righe vuote nel foglio di lavoro devono essere trattate come separatori di tabella durante l'esportazione in Markdown. Il valore predefinito è false.

```csharp
public bool SplitTablesByBlankRow { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertySplitTablesByBlankRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con righe vuote per dimostrare la divisione delle tabelle
            worksheet.Cells["A1"].Value = "Table 1 Header";
            worksheet.Cells["B1"].Value = "Value 1";
            worksheet.Cells["A2"].Value = "Data 1";
            worksheet.Cells["B2"].Value = "Data 2";

            // Aggiungi una riga vuota (riga 3)
            worksheet.Cells["A4"].Value = "Table 2 Header";
            worksheet.Cells["B4"].Value = "Value 2";
            worksheet.Cells["A5"].Value = "Data 3";
            worksheet.Cells["B5"].Value = "Data 4";

            // Crea un'istanza di MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Visualizza il valore predefinito di SplitTablesByBlankRow
                Console.WriteLine("Default SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // Imposta SplitTablesByBlankRow su true per dividere le tabelle per righe vuote
                saveOptions.SplitTablesByBlankRow = true;

                // Visualizza il valore aggiornato
                Console.WriteLine("Updated SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // Salva la cartella di lavoro come markdown con la divisione delle tabelle abilitata
                workbook.Save("SplitTablesByBlankRowDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with table splitting by blank rows enabled.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


