---
title: "Cells.ImportObjectArray"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Importerar en dataarray till ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/cells/importobjectarray/
---
## ImportObjectArray(object[], int, int, bool) {#importobjectarray}

Importerar en matris av data till ett kalkylblad.

```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objArray | Object[] | Dataarray. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |
| ärVertikal | Boolean | Anger om data ska importeras vertikalt eller horisontellt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered en objektarray med exempeldata
            object[] dataArray = new object[] { "Product", "Price", "Stock", "Discontinued", 150.5, 75, false };

            try
            {
                // Importera objektarrayen till kalkylbladet med start i cell B3 (rad 2, kolumn 1), horisontellt
                worksheet.Cells.ImportObjectArray(dataArray, 2, 1, false);

                Console.WriteLine("Object array imported successfully to cells B3:F3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Spara arbetsboken för att demonstrera resultatet
            workbook.Save("CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportObjectArray(object[], int, int, bool, int) {#importobjectarray_1}

Importerar en matris av data till ett kalkylblad.

```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical, 
    int skip)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objArray | Object[] | Dataarray. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |
| ärVertikal | Boolean | Anger om data ska importeras vertikalt eller horisontellt. |
| hoppa över | Int32 | Antal rader eller kolumner som hoppats över. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Förbered data för ImportObjectArray-parametrar: (Object[], Int32, Int32, Boolean, Int32)
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
                // Anropa ImportObjectArray med parametrar: (dataarray, startrad 0, startkolumn 0, horisontell import, hoppa över 1 kolumn mellan poster)
                worksheet.Cells.ImportObjectArray(data, 0, 0, false, 1);
                
                Console.WriteLine("Imported object array with parameters (Object[], 0, 0, false, 1) successfully.");
                
                // Demonstrera effekten: Data kommer att placeras i cellerna A1, C1, E1, A2, C2, E2 osv. med hoppade kolumner
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportObjectArray: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


