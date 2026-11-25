---
title: "ChartGlobalizationSettings.GetAxisTitleName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartGlobalizationSettings. Ottiene il nome del Titolo per l'Asse"
type: docs
url: /it/net/aspose.cells.charts/chartglobalizationsettings/getaxistitlename/
---
## ChartGlobalizationSettings.GetAxisTitleName method

Ottiene il nome del Titolo per l'Asse.

```csharp
public virtual string GetAxisTitleName()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetAxisTitleNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Crea le impostazioni di globalizzazione e ottieni il nome del titolo dell'asse
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string axisTitleName = globalizationSettings.GetAxisTitleName();

            // Imposta il titolo dell'asse
            chart.ValueAxis.Title.Text = axisTitleName;
            chart.CategoryAxis.Title.Text = axisTitleName;

            // Restituisci il nome del titolo dell'asse
            Console.WriteLine("Axis Title Name: " + axisTitleName);

            // Salva la cartella di lavoro
            workbook.Save("ChartGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


