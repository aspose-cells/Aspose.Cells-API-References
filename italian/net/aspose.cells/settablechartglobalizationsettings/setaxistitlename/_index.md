---
title: "SettableChartGlobalizationSettings.SetAxisTitleName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableChartGlobalizationSettings. Imposta il nome del Titolo per l'Asse"
type: docs
url: /it/net/aspose.cells/settablechartglobalizationsettings/setaxistitlename/
---
## SettableChartGlobalizationSettings.SetAxisTitleName method

Imposta il nome del Titolo per l'Asse.

```csharp
public void SetAxisTitleName(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | nome dipendente locale |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetAxisTitleNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati minimi per il contesto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crea un'istanza di SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Imposta un nome personalizzato per il titolo dell'axis
                settings.SetAxisTitleName("Custom Axis Title");

                // Verifica l'impostazione ottenendo il nome del titolo dell'asse
                string axisTitleName = settings.GetAxisTitleName();
                Console.WriteLine("Axis Title Name: " + axisTitleName);

                // Salva la cartella di lavoro
                workbook.Save("SetAxisTitleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetAxisTitleName: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


