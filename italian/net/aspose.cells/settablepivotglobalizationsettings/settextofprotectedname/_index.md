---
title: "SettablePivotGlobalizationSettings.SetTextOfProtectedName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettablePivotGlobalizationSettings. Imposta il testo per un nome protetto specifico"
type: docs
url: /it/net/aspose.cells/settablepivotglobalizationsettings/settextofprotectedname/
---
## SettablePivotGlobalizationSettings.SetTextOfProtectedName method

Imposta il testo per un nome protetto specifico.

```csharp
public void SetTextOfProtectedName(string protectedName, string text)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| protectedName | String | Il nome protetto nella PivotTable. |
| testo | String | I nomi protetti locali della PivotTable. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfProtectedNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio per il contesto
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Crea un'istanza di SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Imposta testo personalizzato per un nome protetto
                settings.SetTextOfProtectedName("Sum", "Custom Sum Label");

                // Verifica la modifica ottenendo il testo corrente
                string currentText = settings.GetTextOfProtectedName("Sum");
                Console.WriteLine($"Text for protected name 'Sum': {currentText}");

                // Salva la cartella di lavoro per dimostrare l'esecuzione corretta
                workbook.Save("SetTextOfProtectedNameDemo.xlsx");
                Console.WriteLine("SetTextOfProtectedName method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


