---
title: "Cells.ImportObjectArray"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Importiert ein Datenarray in ein Arbeitsblatt"
type: docs
url: /de/net/aspose.cells/cells/importobjectarray/
---
## ImportObjectArray(object[], int, int, bool) {#importobjectarray}

Importiert ein Array von Daten in ein Arbeitsblatt.

```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| objArray | Object[] | Datenarray. |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |
| isVertical | Boolean | Gibt an, ob Daten vertikal oder horizontal importiert werden sollen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle ein Objektarray mit Beispieldaten
            object[] dataArray = new object[] { "Product", "Price", "Stock", "Discontinued", 150.5, 75, false };

            try
            {
                // Importiere das Objektarray in das Arbeitsblatt, beginnend bei Zelle B3 (Zeile 2, Spalte 1), horizontal
                worksheet.Cells.ImportObjectArray(dataArray, 2, 1, false);

                Console.WriteLine("Object array imported successfully to cells B3:F3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Speichere die Arbeitsmappe, um die Ausgabe zu demonstrieren
            workbook.Save("CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportObjectArray(object[], int, int, bool, int) {#importobjectarray_1}

Importiert ein Array von Daten in ein Arbeitsblatt.

```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical, 
    int skip)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| objArray | Object[] | Datenarray. |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |
| isVertical | Boolean | Gibt an, ob Daten vertikal oder horizontal importiert werden sollen. |
| überspringen | Int32 | Übersprungene Anzahl von Zeilen oder Spalten. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bereite Daten für die ImportObjectArray-Parameter vor: (Object[], Int32, Int32, Boolean, Int32)
            object[] data = new object[]
            {
                "Name",
                "Age",
                "Date",
                "John Doe",
                30,
                new DateTime(2023, 10, 15),
                "Jane Smith",
                28,
                new DateTime(2023, 10, 16)
            };

            try
            {
                // Rufe ImportObjectArray mit den Parametern auf: (Datenarray, Startzeile 0, Startspalte 0, horizontaler Import, 1 Spalte zwischen Einträgen überspringen)
                worksheet.Cells.ImportObjectArray(data, 0, 0, false, 1);
                
                Console.WriteLine("Imported object array with parameters (Object[], 0, 0, false, 1) successfully.");
                
                // Demonstriere den Effekt: Daten werden in den Zellen A1, C1, E1, A2, C2, E2 usw. mit übersprungenen Spalten platziert
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportObjectArray: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


