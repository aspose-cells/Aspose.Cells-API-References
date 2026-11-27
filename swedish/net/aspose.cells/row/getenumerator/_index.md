---
title: "Row.GetEnumerator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-metod. Hämtar cellernas enumerator"
type: docs
url: /sv/net/aspose.cells/row/getenumerator/
---
## GetEnumerator() {#getenumerator}

Hämtar cellernas enumerator

```csharp
public IEnumerator GetEnumerator()
```

### Returvärde

Cellernas enumerator som kommer att gå igenom alla befintliga celler i den här raden.

### Exempel

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fyll i lite exempeldata
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            // Hämta enumerator för första raden (rubrikrad)
            IEnumerator en = cells.Rows[0].GetEnumerator();
            while (en.MoveNext())
            {
                Cell cell = (Cell)en.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }
        }
    }
}
```

### Se även

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

Hämtar en enumerator som itererar celler genom den här raden.

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| omvänd | Boolean | om celler ska enumereras i omvänd ordning |
| synk | Boolean | om den returnerade enumeratorn ska kontrollera ändringar av celler i den här raden och hålla sig synkroniserad med den. |

### Returvärde

Cellernas enumerator som kommer att gå igenom alla befintliga celler i den här raden.

### Anmärkningar

Om raden kommer att modifieras (genom operationer som kan orsaka att en ny Cell instansieras eller en befintlig Cell tas bort) under traverseringen med enumeratorn, bör en synkroniserad enumerator användas istället för en normal enumerator så att traverseringen kan fortsätta från positionen precis efter den som har traverserats av den senaste MoveNext(). Dock, förutom fördelen att inget element hoppar över eller traverseras flera gånger, är nackdelen med den synkroniserade enumeratorn att prestandan blir något försämrad jämfört med en normal enumerator.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i celler i första raden
            Row row = worksheet.Cells.Rows[0];
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            try
            {
                // Anropa GetEnumerator med reversed=false och sync=true
                IEnumerator enumerator = row.GetEnumerator(false, true);
                
                Console.WriteLine("Cells in row 1:");
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }

                // Anropa GetEnumerator med reversed=true och sync=false för att demonstrera omvänd iteration
                Console.WriteLine("\nCells in row 1 (reversed order):");
                enumerator = row.GetEnumerator(true, false);
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("RowMethodGetEnumeratorWithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Se även

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


