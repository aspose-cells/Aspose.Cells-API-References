---
title: "LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LowCodeSaveOptionsProviderOfAssembling. Ottiene le opzioni di salvataggio da cui ricavare le impostazioni di output per la parte attualmente divisa"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/
---
## LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions method

Ottiene le opzioni di salvataggio da cui ricavare le impostazioni di output per la parte divisa corrente.

```csharp
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingMethodGetSaveOptionsWithSplitPartInfoDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].Value = "Sample Data for Split";

            try
            {
                // Crea un'istanza di LowCodeSaveOptionsProviderOfAssembling
                var provider = new LowCodeSaveOptionsProviderOfAssembling
                {
                    PathHeader = "Output/",
                    PathTail = ".xlsx",
                    UseSheetName = true,
                    SheetPrefix = "Sheet_",
                    SplitPartPrefix = "Part_",
                    SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
                };

                // Crea un'istanza di SplitPartInfo usando la riflessione poiché il costruttore non è accessibile
                var splitPartInfo = (SplitPartInfo)Activator.CreateInstance(typeof(SplitPartInfo), nonPublic: true);

                // Chiama GetSaveOptions con il parametro SplitPartInfo
                LowCodeSaveOptions saveOptions = provider.GetSaveOptions(splitPartInfo);

                Console.WriteLine("SaveOptions created successfully");
                Console.WriteLine($"Output format: {saveOptions.SaveFormat}");

                // Salva la cartella di lavoro (in un utilizzo reale questo userebbe le opzioni di salvataggio generate)
                workbook.Save("GetSaveOptionsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in GetSaveOptions demo: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


