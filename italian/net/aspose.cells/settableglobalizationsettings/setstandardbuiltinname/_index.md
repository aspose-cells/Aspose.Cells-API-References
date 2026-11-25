---
title: "SettableGlobalizationSettings.SetStandardBuiltInName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Imposta il nome della funzione dipendente dalla locale secondo il nome della funzione standard fornito"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/setstandardbuiltinname/
---
## SettableGlobalizationSettings.SetStandardBuiltInName method

Imposta il nome della funzione dipendente dalla locale secondo il nome della funzione standard fornito.

```csharp
public void SetStandardBuiltInName(string localName, string standardName, bool bidirectional)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| localName | String | Nome della funzione dipendente dalla locale |
| standardName | String | Nome della funzione Standard (locale en-US). |
| bidirectional | Boolean | Se mappare automaticamente il testo del nome standard al testo del nome locale. Se vero, il testo del nome standard verrà mappato al testo del nome locale automaticamente così l'utente non deve chiamare nuovamente [`SetLocalBuiltInName`](../setlocalbuiltinname/) per la stessa coppia di nomi standard e locale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardBuiltInNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Imposta le impostazioni di globalizzazione per la cartella di lavoro
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Chiama SetStandardBuiltInName per mappare un nome locale a un nome standard incorporato
                // Parametri: localName, standardName, bidirectional
                settings.SetStandardBuiltInName("MyLocalName", "SUM", true);
                
                Console.WriteLine("SetStandardBuiltInName executed successfully with parameters (\"MyLocalName\", \"SUM\", true)");
                
                // Dimostra l'effetto usando il nome locale in una formula
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=MyLocalName(A1:A2)";
                
                // Calcola la formula per mostrare che funziona con il nome locale
                workbook.CalculateFormula();
                Console.WriteLine("Result of formula with local name: " + worksheet.Cells["A3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardBuiltInName method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("SetStandardBuiltInNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


