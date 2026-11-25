---
title: "SettableChartGlobalizationSettings.GetAxisUnitName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableChartGlobalizationSettings. Ottiene il Nome dell'Unità dell'Asse"
type: docs
url: /it/net/aspose.cells/settablechartglobalizationsettings/getaxisunitname/
---
## SettableChartGlobalizationSettings.GetAxisUnitName method

Ottiene il nome dell'Unità dell'Asse.

```csharp
public override string GetAxisUnitName(DisplayUnitType type)
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetAxisUnitNameWithDisplayUnitTypeDemo
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

                // Chiama GetAxisUnitName con valori diversi di DisplayUnitType
                string hundredsUnit = settings.GetAxisUnitName(DisplayUnitType.Hundreds);
                string thousandsUnit = settings.GetAxisUnitName(DisplayUnitType.Thousands);
                string millionsUnit = settings.GetAxisUnitName(DisplayUnitType.Millions);
                string percentageUnit = settings.GetAxisUnitName(DisplayUnitType.Percentage);

                // Visualizza i risultati
                Console.WriteLine($"Hundreds unit name: {hundredsUnit}");
                Console.WriteLine($"Thousands unit name: {thousandsUnit}");
                Console.WriteLine($"Millions unit name: {millionsUnit}");
                Console.WriteLine($"Percentage unit name: {percentageUnit}");

                // Salva la cartella di lavoro
                workbook.Save("GetAxisUnitNameDemo.xlsx");
                Console.WriteLine("GetAxisUnitName method called successfully. Workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetAxisUnitName: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [DisplayUnitType](../../../aspose.cells.charts/displayunittype/)
* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


