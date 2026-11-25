---
title: "LowCodeSaveOptionsProviderOfAssembling.UseSheetName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSaveOptionsProviderOfAssembling. Indica se costruisce il percorso del file con il nome del foglio invece dell'indice del foglio. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/
---
## LowCodeSaveOptionsProviderOfAssembling.UseSheetName property

Indica se costruire il percorso del file con il nome del foglio invece dell'indice del foglio. Il valore predefinito è false.

```csharp
public bool UseSheetName { get; set; }
```

### Osservazioni

Il nome del foglio non verrà mai ricostruito automaticamente. Quindi, quando lo imposti su true, assicurati che non ci siano nomi di foglio speciali che possano causare percorsi o nomi di file non validi.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyUseSheetNameDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con un foglio di lavoro denominato
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "MonthlyReport";
            
            // Aggiungi dati di esempio per la dimostrazione della divisione
            for(int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Record {i+1}");
            }

            // Crea e configura il provider
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "split_files/",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet_",
                SplitPartPrefix = "Part_",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Dimostra UseSheetName=false (predefinito)
            Console.WriteLine($"Default UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_default", provider.SaveOptionsTemplate.SaveFormat);

            // Modifica la proprietà e dimostra il nuovo comportamento
            provider.UseSheetName = true;
            Console.WriteLine($"\nModified UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_modified", provider.SaveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check 'split_files' directory for output files with different naming schemes");
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


