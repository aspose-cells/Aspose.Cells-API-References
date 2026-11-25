---
title: "SettableChartGlobalizationSettings.GetOtherName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableChartGlobalizationSettings. Ottiene il nome delle etichette Other per il Chart"
type: docs
url: /it/net/aspose.cells/settablechartglobalizationsettings/getothername/
---
## SettableChartGlobalizationSettings.GetOtherName method

Ottiene il nome delle etichette "Altro" per il Grafico.

```csharp
public override string GetOtherName()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetOtherNameDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati minimi (opzionale, solo per un workbook completo)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(250);

            try
            {
                // Istanzia l'oggetto delle impostazioni di globalizzazione
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Imposta un nome personalizzato per l'etichetta "Other"
                settings.SetOtherName("Custom Other Label");

                // Recupera il nome usando GetOtherName
                string otherName = settings.GetOtherName();

                Console.WriteLine("Other Name retrieved: " + otherName);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetOtherName: {ex.Message}");
            }

            // Salva il workbook (le impostazioni non sono direttamente collegate al chart in questa demo)
            workbook.Save("GetOtherNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


