---
title: "LightCellsDataHandler.ProcessRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LightCellsDataHandler-Methode. Beginnt mit der Verarbeitung einer Zeile"
type: docs
url: /de/net/aspose.cells/lightcellsdatahandler/processrow/
---
## LightCellsDataHandler.ProcessRow method

Beginnt mit der Verarbeitung einer Zeile.

```csharp
public bool ProcessRow(Row row)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Row | Zeilenobjekt, das gerade verarbeitet wird. |

### Rückgabewert

Ob die Zellen dieser Zeile verarbeitet werden müssen. false, um alle Zellen in dieser Zeile zu ignorieren.

### Hinweise

Sie wird aufgerufen, nachdem die Eigenschaften der Zeile wie Höhe, Stil, ...etc. gelesen wurden. Die Zellen dieser Zeile wurden jedoch noch nicht gelesen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerMethodProcessRowWithRowDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Fügen Sie Beispieldaten hinzu
                worksheet.Cells["A1"].Value = "Test Data";
                worksheet.Cells["A2"].Value = 100;
                worksheet.Cells["B2"].Value = 200;

                // Benutzerdefinierten Handler erstellen
                var handler = new CustomRowHandler();

                // Erste Zeile verarbeiten
                Row firstRow = worksheet.Cells.Rows[0];
                bool result = handler.ProcessRow(firstRow);

                Console.WriteLine($"ProcessRow returned: {result}");
                Console.WriteLine($"Row height after processing: {firstRow.Height}");

                workbook.Save("ProcessRowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ProcessRow demo: {ex.Message}");
            }
        }

        private class CustomRowHandler : LightCellsDataHandler
        {
            public bool ProcessRow(Row row)
            {
                // Demonstration des Zugriffs auf Zeileneigenschaften
                Console.WriteLine($"Processing row index: {row.Index}");
                Console.WriteLine($"Row is hidden: {row.IsHidden}");
                Console.WriteLine($"Row is blank: {row.IsBlank}");

                // Zeilenhöhe ändern, wenn es nicht die Kopfzeile ist
                if (row.Index > 0)
                {
                    row.Height = 25.0;
                }

                return true;
            }

            public bool StartSheet(Worksheet sheet) => true;
            public bool StartRow(int rowIndex) => true;
            public bool StartCell(int columnIndex) => true;
            public bool ProcessCell(Cell cell) => true;
        }
    }
}
```

### Siehe auch

* class [Row](../../row/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


