---
title: "Aufzählung FilterCategory"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FilterCategory Aufzählung. Stellt die Kategorie des Filters dar"
type: docs
url: /de/net/aspose.cells/filtercategory/
---
## FilterCategory enumeration

Stellt die Kategorie des Filters dar.

```csharp
public enum FilterCategory
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Kein Filter. |
| Label | `1` | Beschriftungsfilter. |
| NumberValue | `2` | Zahlenwertfilter. |
| Date | `3` | Datumswertfilter. |
| Top10 | `4` | Top‑10‑Wertfilter. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class CellsClassFilterCategoryDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            CreateSampleData(worksheet);

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:C7", "H5");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Zeilenfelder konfigurieren
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            
            // Datenfeld konfigurieren
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Beschriftungsfilter zu Pivot-Filtern hinzufügen
            PivotFilter filter = pivotTable.PivotFilters.AddLabelFilter(0, PivotFilterType.CaptionEqual, "East", null);
            
            // Verwendung von FilterCategory demonstrieren
            Console.WriteLine("Filter Category: " + filter.FilterCategory);
            
            // Alle Filterkategorien in der Pivot-Tabelle anzeigen
            foreach (PivotFilter pivotFilter in pivotTable.PivotFilters)
            {
                Console.WriteLine($"Filter Type: {pivotFilter.FilterType}, Category: {pivotFilter.FilterCategory}");
            }

            // Pivot-Tabelle aktualisieren und berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Ergebnis speichern
            workbook.Save("FilterCategoryDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Beispiel-Datenkopfzeilen festlegen
            worksheet.Cells["A1"].Value = "Region";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";

            // Beispiel-Datenzeilen hinzufügen
            object[,] data = new object[,]
            {
                {"East", "Apples", 5000},
                {"West", "Oranges", 3000},
                {"East", "Bananas", 4000},
                {"North", "Apples", 6000},
                {"South", "Oranges", 2000},
                {"East", "Bananas", 4500},
                {"West", "Apples", 5500}
            };

            int rowCount = data.GetLength(0);
            int colCount = data.GetLength(1);

            for (int i = 0; i < rowCount; i++)
            {
                for (int j = 0; j < colCount; j++)
                {
                    worksheet.Cells[i + 2, j].Value = data[i, j];
                }
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


