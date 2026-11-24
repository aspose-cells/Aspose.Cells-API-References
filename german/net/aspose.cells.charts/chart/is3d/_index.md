---
title: "Chart.Is3D"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Gibt an, ob das Diagramm ein 3D-Diagramm ist"
type: docs
url: /de/net/aspose.cells.charts/chart/is3d/
---
## Chart.Is3D property

Gibt an, ob das Diagramm ein 3‑D‑Diagramm ist.

```csharp
public bool Is3D { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertyIs3DDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Datenbereich für das Diagramm festlegen
            chart.SetChartDataRange("A1:B5", true);

            // Zeigen Sie den aktuellen Is3D-Wert an
            Console.WriteLine("Current Is3D value: " + chart.Is3D);

            // Erstellen Sie eine 3D-Version des Diagramms
            int chart3DIndex = worksheet.Charts.Add(ChartType.Column3D, 6, 12, 20, 22);
            Chart chart3D = worksheet.Charts[chart3DIndex];
            chart3D.SetChartDataRange("A1:B5", true);

            // Zeigen Sie den Is3D-Wert des 3D-Diagramms an
            Console.WriteLine("3D Chart Is3D value: " + chart3D.Is3D);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPropertyIs3DDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


