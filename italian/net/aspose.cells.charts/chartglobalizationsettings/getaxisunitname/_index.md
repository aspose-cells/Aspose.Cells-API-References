---
title: "ChartGlobalizationSettings.GetAxisUnitName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartGlobalizationSettings. Ottiene il Nome dell'Unità dell'Asse"
type: docs
url: /it/net/aspose.cells.charts/chartglobalizationsettings/getaxisunitname/
---
## ChartGlobalizationSettings.GetAxisUnitName method

Ottiene il nome dell'Unità dell'Asse.

```csharp
public virtual string GetAxisUnitName(DisplayUnitType type)
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetAxisUnitNameWithDisplayUnitTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Crea le impostazioni di globalizzazione e ottieni il nome dell'unità dell'asse
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string thousandsUnit = globalizationSettings.GetAxisUnitName(DisplayUnitType.Thousands);
            string millionsUnit = globalizationSettings.GetAxisUnitName(DisplayUnitType.Millions);

            // Restituisci i risultati
            Console.WriteLine("Thousands unit name: " + thousandsUnit);
            Console.WriteLine("Millions unit name: " + millionsUnit);

            // Salva cartella di lavoro
            workbook.Save("AxisUnitNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [DisplayUnitType](../../displayunittype/)
* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


