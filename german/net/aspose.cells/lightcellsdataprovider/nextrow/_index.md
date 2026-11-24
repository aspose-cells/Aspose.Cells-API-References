---
title: "LightCellsDataProvider.NextRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LightCellsDataProvider‑Methode. Gibt die nächste zu speichernde Zeile zurück"
type: docs
url: /de/net/aspose.cells/lightcellsdataprovider/nextrow/
---
## LightCellsDataProvider.NextRow method

Ermittelt die nächste zu speichernde Zeile.

```csharp
public int NextRow()
```

### Rückgabewert

Der Index der nächsten zu speichernden Zeile. -1 bedeutet, dass das Ende der aktuellen Blattdaten erreicht ist und keine weitere Zeile des aktuellen Blatts gespeichert werden muss.

### Hinweise

Wird zu Beginn des Speicherns einer Zeile und ihrer Zellen-Daten aufgerufen (vor [`StartRow`](../startrow/)).

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodNextRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            workbook.Worksheets.Add("Sheet1");

            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();

            try
            {
                workbook.Save("LightCellsDataProviderMethodNextRowDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with LightCellsDataProvider implementation.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private int currentRow = -1;
        private int currentCell = -1;
        private readonly int totalRows = 3;

        public bool StartSheet(int sheetIndex)
        {
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            currentRow++;
            currentCell = -1;
            return currentRow < totalRows ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            row.Height = 20;
        }

        public int NextCell()
        {
            currentCell++;
            return currentCell < 2 ? currentCell : -1;
        }

        public void StartCell(Cell cell)
        {
            cell.PutValue($"R{currentRow}C{currentCell}");
        }

        public bool IsGatherString()
        {
            return false;
        }
    }
}
```

### Siehe auch

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


