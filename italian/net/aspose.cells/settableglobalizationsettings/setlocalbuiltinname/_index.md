---
title: "SettableGlobalizationSettings.SetLocalBuiltInName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Imposta il testo dipendente dalla locale per il nome incorporato con il testo del nome standard fornito"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/setlocalbuiltinname/
---
## SettableGlobalizationSettings.SetLocalBuiltInName method

Imposta il testo dipendente dalla locale per il nome integrato con il testo del nome standard fornito.

```csharp
public void SetLocalBuiltInName(string standardName, string localName, bool bidirectional)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| standardName | String | Testo del nome standard (locale en-US) del nome incorporato. |
| localName | String | Testo del nome dipendente dalla locale |
| bidirectional | Boolean | Indica se mappare automaticamente il testo del nome locale al testo del nome standard. Se vero, il testo del nome locale verrà mappato al testo del nome standard automaticamente così l'utente non deve chiamare nuovamente [`SetStandardBuiltInName`](../setstandardbuiltinname/) per la stessa coppia di nomi standard e locale |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalBuiltInNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Chiama SetLocalBuiltInName per mappare un nome incorporato standard a un nome locale
                settings.SetLocalBuiltInName("SUM", "LOCAL_SUM", true);

                // Applica le impostazioni alla cartella di lavoro
                workbook.Settings.GlobalizationSettings = settings;

                // Crea una formula usando il nome incorporato standard
                worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 5;
                worksheet.Cells["B2"].Value = 10;
                worksheet.Cells["B3"].Value = 15;

                // Calcola la formula
                workbook.CalculateFormula();

                Console.WriteLine("Formula with standard built-in name 'SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");

                // Verifica la mappatura del nome locale
                string localName = settings.GetLocalBuiltInName("SUM");
                Console.WriteLine($"Local name for 'SUM': {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalBuiltInName method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("SetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


