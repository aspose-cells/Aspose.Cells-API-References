---
title: "WorksheetCollection.GetRangeByName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Methode. Gibt ein Range-Objekt anhand eines vordefinierten Namens zurück"
type: docs
url: /de/net/aspose.cells/worksheetcollection/getrangebyname/
---
## GetRangeByName(string) {#getrangebyname}

Ruft das Range‑Objekt über einen vordefinierten Namen ab.

```csharp
public Range GetRangeByName(string rangeName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rangeName | String | Name des Bereichs. |

### Rückgabewert

Range-Objekt.

Gibt null zurück, wenn der benannte Bereich nicht existiert.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetRangeByNameWithStringDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Daten zu den Zellen hinzufügen
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["B1"].PutValue("Banana");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            
            // Benannten Bereich erstellen
            worksheet.Cells.CreateRange("A1:B2").Name = "FruitData";
            
            // Rufen Sie den benannten Bereich mit GetRangeByName ab
            Aspose.Cells.Range namedRange = workbook.Worksheets.GetRangeByName("FruitData");
            
            // Bereichsinformationen anzeigen, falls gefunden
            if (namedRange != null)
            {
                Console.WriteLine("Range found: " + namedRange.Address);
                Console.WriteLine("First cell value: " + namedRange[0, 0].StringValue);
            }
            else
            {
                Console.WriteLine("Range not found");
            }
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRangeByName(string, int, bool) {#getrangebyname_1}

Ruft [`Range`](../../range/) über vordefinierten Namen oder Tabellennamen ab

```csharp
public Range GetRangeByName(string rangeName, int currentSheetIndex, bool includeTable)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rangeName | String | Name des Bereichs oder Tabellenname. |
| currentSheetIndex | Int32 | Der Blattindex. -1 steht für global. |
| includeTable | Boolean | Gibt an, ob alle Tabellen geprüft werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodGetRangeByNameWithStringInt32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Benannten Bereich erstellen
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("A1", "C3");
            namedRange.Name = "TestRange";
            
            // Fügen Sie dem Bereich einige Daten hinzu
            for (int i = 0; i < 3; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            try
            {
                // Rufen Sie GetRangeByName mit den Parametern (String, Int32, Boolean) auf
                Aspose.Cells.Range retrievedRange = workbook.Worksheets.GetRangeByName("TestRange", 0, true);
                
                Console.WriteLine("Method executed successfully with parameters (String, Int32, Boolean)");
                Console.WriteLine($"Retrieved range address: {retrievedRange.Address}");
                Console.WriteLine($"Range contains {retrievedRange.RowCount} rows and {retrievedRange.ColumnCount} columns");
                
                // Bereichswerte anzeigen
                Console.WriteLine("Range values:");
                foreach (Cell cell in retrievedRange)
                {
                    Console.WriteLine($"{cell.Name}: {cell.Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRangeByName method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("WorksheetCollectionMethodGetRangeByNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


