---
title: "SettableGlobalizationSettings.GetStandardBuiltInName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Ottiene il testo standard del Nome incorporato in base al testo dipendente dalla locale fornito"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/getstandardbuiltinname/
---
## SettableGlobalizationSettings.GetStandardBuiltInName method

Ottiene il testo standard del Nome incorporato in base al testo dipendente dalla locale fornito.

```csharp
public override string GetStandardBuiltInName(string localName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| localName | String | Testo dipendente dalla locale del Nome incorporato. La locale è stata specificata dalla Cartella di lavoro per la quale queste impostazioni sono utilizzate. |

### Valore di ritorno

Testo standard (locale en-US).

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            // Imposta un nome incorporato locale per la dimostrazione
            globalizationSettings.SetLocalBuiltInName("SUM", "LocalSumName", true);

            try
            {
                // Chiama il metodo GetStandardBuiltInName con un nome locale
                string standardName = globalizationSettings.GetStandardBuiltInName("LocalSumName");
                
                // Visualizza il risultato
                Console.WriteLine($"Standard name for 'LocalSumName' is: {standardName}");

                // Applica il risultato a una cella
                worksheet.Cells["A1"].Formula = "=" + standardName + "(1,2,3)";
                workbook.CalculateFormula();

                // Visualizza il risultato calcolato
                Console.WriteLine($"Result of formula in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


