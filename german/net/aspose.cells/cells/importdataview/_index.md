---
title: "Cells.ImportDataView"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Importiert ein DataView in ein Arbeitsblatt."
type: docs
url: /de/net/aspose.cells/cells/importdataview/
---
## Cells.ImportDataView method

Importiert ein DataView in ein Arbeitsblatt.

```csharp
public int ImportDataView(DataView dataView, int firstRow, int firstColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataView | DataView | Das zu importierende DataView-Objekt. |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |

### Rückgabewert

Gesamtzahl der importierten Zeilen

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataViewWithDataViewInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispiel-DataTable erstellen.
            DataTable table = new DataTable("Products");
            table.Columns.Add("ID", typeof(int));
            table.Columns.Add("Name", typeof(string));
            table.Columns.Add("Price", typeof(decimal));

            // Fügen Sie Beispieldaten hinzu
            table.Rows.Add(1, "Laptop", 999.99m);
            table.Rows.Add(2, "Smartphone", 699.99m);
            table.Rows.Add(3, "Tablet", 399.99m);

            // DataView aus DataTable erstellen.
            DataView dataView = new DataView(table);

            // Importiere DataView in ein Arbeitsblatt, beginnend bei Zeile 0, Spalte 0.
            cells.ImportDataView(dataView, 0, 0);

            // Speichere die Arbeitsmappe
            workbook.Save("ImportDataViewOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


