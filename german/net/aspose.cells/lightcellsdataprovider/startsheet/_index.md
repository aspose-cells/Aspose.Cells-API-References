---
title: "LightCellsDataProvider.StartSheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LightCellsDataProvider‑Methode. Beginnt mit dem Speichern eines Arbeitsblatts"
type: docs
url: /de/net/aspose.cells/lightcellsdataprovider/startsheet/
---
## LightCellsDataProvider.StartSheet method

Beginnt, ein Arbeitsblatt zu speichern.

```csharp
public bool StartSheet(int sheetIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | Int32 | Index des zu speichernden aktuellen Arbeitsblatts. |

### Rückgabewert

true, wenn dieser Provider Daten für das angegebene Arbeitsblatt bereitstellt; false, wenn das angegebene Arbeitsblatt sein normales Datenmodell (Cells) verwenden soll.

### Hinweise

Wird zu Beginn des Speicherns eines Arbeitsblatts während des Speicherns einer Arbeitsmappe aufgerufen. Wenn der Provider darauf verweisen muss

```csharp
sheetIndex
```

später in der startRow(Row)- oder startCell(Cell)-Methode, das heißt, wenn der Prozess wissen muss, welches Arbeitsblatt verarbeitet wird, sollte die Implementierung das

```csharp
sheetIndex
```

hier den Wert.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartSheetWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                Workbook workbook = new Workbook();
                workbook.Worksheets.Clear(); // Start with clean worksheet
                
                // Erstelle einen benutzerdefinierten Datenprovider und speichere im Light‑Cells‑Modus
                var saveOptions = new OoxmlSaveOptions
                {
                    LightCellsDataProvider = new CustomLightCellsDataProvider()
                };

                Console.WriteLine("Starting workbook save with LightCellsDataProvider...");
                workbook.Save("StartSheetDemoOutput.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully. Check StartSheetDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private bool sheetProcessed = false;

            // Wird aufgerufen, wenn ein Arbeitsblatt verarbeitet wird
            public bool StartSheet(int sheetIndex)
            {
                Console.WriteLine($"Processing sheet index: {sheetIndex}");
                // Nur das erste Arbeitsblatt verarbeiten (Index 0)
                if (sheetIndex == 0)
                {
                    sheetProcessed = true;
                    return true;
                }
                return false;
            }

            public int NextRow()
            {
                if (sheetProcessed)
                {
                    sheetProcessed = false;
                    return 0; // Process first row (index 0)
                }
                return -1; // Stop processing after first row
            }

            public void StartRow(Row row)
            {
                row.Height = 20;
            }

            public int NextCell()
            {
                return 0; // Process first cell (index 0)
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue("Data from LightCellsDataProvider");
            }

            public bool IsGatherString()
            {
                return false;
            }
        }
    }
}
```

### Siehe auch

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


