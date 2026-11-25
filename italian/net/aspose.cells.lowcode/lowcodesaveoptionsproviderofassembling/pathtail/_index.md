---
title: "LowCodeSaveOptionsProviderOfAssembling.PathTail"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSaveOptionsProviderOfAssembling. Parte finale dopo i numeri di sequenza del percorso del file. Deve includere l'estensione del nome del file"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathtail/
---
## LowCodeSaveOptionsProviderOfAssembling.PathTail property

Parte finale (dopo i numeri di sequenza) del percorso del file. Deve includere l'estensione del nome file.

```csharp
public string PathTail { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyPathTailDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 25; i++)
            {
                worksheet.Cells[i, 0].Value = $"Record {i + 1}";
            }

            // Inizializza il provider delle opzioni di salvataggio
            var optionsProvider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SalesReports/Q3",
                PathTail = ".xlsx",
                UseSheetName = true,
                SaveOptionsTemplate = new LowCodeSaveOptions
                {
                    SaveFormat = SaveFormat.Xlsx
                }
            };

            Console.WriteLine($"Original file extension: {optionsProvider.PathTail}");

            // Primo salvataggio con estensione predefinita
            workbook.Save("output_original", optionsProvider.SaveOptionsTemplate.SaveFormat);

            // Modifica la parte finale del percorso per l'output CSV
            optionsProvider.PathTail = "_split.csv";
            optionsProvider.SaveOptionsTemplate.SaveFormat = SaveFormat.Csv;
            Console.WriteLine($"Modified file extension: {optionsProvider.PathTail}");

            // Secondo salvataggio con nuova estensione
            workbook.Save("output_modified", optionsProvider.SaveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check output directories for generated file formats");
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


