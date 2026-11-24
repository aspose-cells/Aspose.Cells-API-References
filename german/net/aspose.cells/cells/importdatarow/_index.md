---
title: "Cells.ImportDataRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Importiert ein DataRow in die Excel-Datei"
type: docs
url: /de/net/aspose.cells/cells/importdatarow/
---
## Cells.ImportDataRow method

Importiert ein DataRow in die Excel-Datei.

```csharp
public void ImportDataRow(DataRow dataRow, int row, int firstColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataRow | DataRow | DataRow-Objekt. |
| row | Int32 | Zeilenindex. |
| firstColumn | Int32 | Erster Spaltenindex. |

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataRowWithDataRowInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Erstelle ein Beispiel-DataTable
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // Fügen Sie Beispieldaten hinzu
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // Importiere die erste Zeile aus DataTable in das Arbeitsblatt, beginnend bei Zeile 0, Spalte 0
            cells.ImportDataRow(dataTable.Rows[0], 0, 0);

            // Speichere die Arbeitsmappe
            workbook.Save("ImportDataRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


