---
title: "ImportTableOptions.TotalColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImportTableOptions-Eigenschaft. Gibt die Gesamtanzahl der zu importierenden Spalten aus der Datenquelle zurück oder legt sie fest. 1 bedeutet alle Zeilen der angegebenen Datenquelle"
type: docs
url: /de/net/aspose.cells/importtableoptions/totalcolumns/
---
## ImportTableOptions.TotalColumns property

Liest oder legt die Gesamtanzahl der zu importierenden Spalten aus der Datenquelle fest. -1 bedeutet, dass alle Zeilen der angegebenen Datenquelle importiert werden.

```csharp
public int TotalColumns { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalColumnsDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispiel-DataTable
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // Fügen Sie Beispieldaten hinzu
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Importoptionen mit TotalColumns = 2 festlegen (es werden nur die ersten 2 Spalten importiert)
            ImportTableOptions importOptions = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalColumns = 2 // Only import first 2 columns (ID and Name)
            };

            // Daten ab Zelle A1 importieren
            cells.ImportData(dataTable, 0, 0, importOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("ImportWithTotalColumns.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Data imported with TotalColumns=2. Only first 2 columns were imported.");
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


