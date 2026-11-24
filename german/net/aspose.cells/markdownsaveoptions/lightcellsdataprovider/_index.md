---
title: "MarkdownSaveOptions.LightCellsDataProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MarkdownSaveOptions-Eigenschaft. Der Datenanbieter, der Zellen‑Daten zum Speichern der Arbeitsmappe im Light‑Modus bereitstellt"
type: docs
url: /de/net/aspose.cells/markdownsaveoptions/lightcellsdataprovider/
---
## MarkdownSaveOptions.LightCellsDataProvider property

Der Datenanbieter, der Zellen­daten zum Speichern der Arbeitsmappe im Light‑Modus bereitstellt.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections.Generic;

    public class MarkdownSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Beispieldaten einfügen
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = "Item " + (i + 1);
                worksheet.Cells[i, 1].Value = i + 1;
            }

            // Benutzerdefinierten LightCellsDataProvider erstellen
            var dataProvider = new CustomLightCellsDataProvider();

            // MarkdownSaveOptions erstellen
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            
            // Aktuellen Wert anzeigen (sollte zunächst null sein)
            Console.WriteLine("Current LightCellsDataProvider value: " + (saveOptions.LightCellsDataProvider == null ? "null" : "set"));

            // Den benutzerdefinierten Datenanbieter festlegen
            saveOptions.LightCellsDataProvider = dataProvider;

            // Mit dem benutzerdefinierten Datenanbieter speichern
            workbook.Save("LightCellsDataProviderDemo.md", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private List<string> items = new List<string> { "Apple", "Banana", "Cherry", "Date", "Elderberry" };
        private List<double> values = new List<double> { 1.99, 0.99, 2.99, 3.49, 4.99 };
        private int currentRow = -1;

        public bool StartSheet(int sheetIndex)
        {
            // Nur das erste Blatt verarbeiten
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            currentRow++;
            return currentRow < items.Count ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            // Zeilenhöhe bei Bedarf festlegen
            row.Height = 15;
        }

        public int NextCell()
        {
            if (currentRow == -1)
            {
                // Kopfzeile
                return currentRow < 2 ? currentRow + 1 : -1;
            }
            else
            {
                return currentRow < 2 ? currentRow + 1 : -1;
            }
        }

        public void StartCell(Cell cell)
        {
            if (currentRow == -1)
            {
                // Kopfzeile
                if (cell.Column == 0)
                    cell.Value = "Product";
                else if (cell.Column == 1)
                    cell.Value = "Price";
            }
            else
            {
                // Daten
                if (cell.Column == 0)
                    cell.Value = items[currentRow];
                else if (cell.Column == 1)
                    cell.Value = values[currentRow];
            }
        }

        public bool IsGatherString()
        {
            return false;
        }
    }
}
```

### Siehe auch

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


