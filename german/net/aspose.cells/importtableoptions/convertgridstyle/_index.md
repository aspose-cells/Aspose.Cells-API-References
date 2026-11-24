---
title: "ImportTableOptions.ConvertGridStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImportTableOptions-Eigenschaft. Gibt an, ob der Stil der Grid-Ansicht auf Zellen angewendet wird"
type: docs
url: /de/net/aspose.cells/importtableoptions/convertgridstyle/
---
## ImportTableOptions.ConvertGridStyle property

Gibt an, ob der Stil der Grid-Ansicht auf Zellen angewendet wird.

```csharp
public bool ConvertGridStyle { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyConvertGridStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle Beispieldaten
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            dataTable.Rows.Add(101, "Laptop", 999.99m);
            dataTable.Rows.Add(102, "Monitor", 249.50m);

            // Importoptionen festlegen, wobei ConvertGridStyle aktiviert ist
            ImportTableOptions options = new ImportTableOptions();
            options.ConvertGridStyle = true; // This will apply grid styling to the imported data
            options.IsFieldNameShown = true;

            // Daten mit Formatierung importieren
            worksheet.Cells.ImportData(dataTable, 0, 0, options);

            // Ergebnis speichern
            workbook.Save("ImportWithGridStyle.xlsx");
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


