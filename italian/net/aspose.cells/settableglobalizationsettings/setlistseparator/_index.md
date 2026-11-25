---
title: "SettableGlobalizationSettings.SetListSeparator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Imposta il separatore per i parametri di elenco della funzione ...etc"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/setlistseparator/
---
## SettableGlobalizationSettings.SetListSeparator method

Imposta il separatore per l'elenco, i parametri della funzione, ...ecc.

```csharp
public void SetListSeparator(char c)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| c | Carattere | il separatore specificato |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetListSeparatorWithCharDemo
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
                // Chiama il metodo SetListSeparator con un parametro di tipo carattere
                settings.SetListSeparator(';');
                
                // Applica le impostazioni alla cartella di lavoro
                workbook.Settings.GlobalizationSettings = settings;
                
                // Dimostra l'effetto creando una formula con il separatore di elenco
                worksheet.Cells["A1"].Formula = "SUM(1;2;3)";
                worksheet.Cells["A2"].Value = "Formula using custom list separator: SUM(1;2;3)";
                
                Console.WriteLine("SetListSeparator method executed successfully with parameter ';'");
                Console.WriteLine("Formula using custom list separator created in cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetListSeparator method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("SetListSeparatorWithCharDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


