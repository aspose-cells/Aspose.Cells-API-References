---
title: "RowCollection.GetEnumerator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RowCollection‑metod. Hämtar en enumerator som itererar rader genom denna samling"
type: docs
url: /sv/net/aspose.cells/rowcollection/getenumerator/
---
## GetEnumerator() {#getenumerator}

Hämtar en enumerator som itererar rader genom denna samling

```csharp
public IEnumerator GetEnumerator()
```

### Returvärde

Rad‑enumeratorn som kommer att gå igenom alla befintliga rader i denna samling.

### Exempel

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in radhöjder för demonstration
            worksheet.Cells.SetRowHeight(0, 15);
            worksheet.Cells.SetRowHeight(1, 20);
            worksheet.Cells.SetRowHeight(2, 25);

            IEnumerator enumerator = worksheet.Cells.Rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine($"Row index: {row.Index}, Height: {row.Height}");
            }
        }
    }
}
```

### Se även

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

Hämtar en enumerator som itererar rader genom denna samling

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| omvänd | Boolean | om rader ska enumereras i omvänd ordning |
| synk | Boolean | om den returnerade enumeratorn ska kontrollera ändringar i radkollektionen och hålla sig synkroniserad med den. |

### Returvärde

Rad‑enumeratorn som kommer att gå igenom alla befintliga rader i denna samling.

### Anmärkningar

Om radkollektionen kommer att modifieras (genom operationer som kan leda till att en ny Rad skapas eller en befintlig Rad tas bort) under traverseringen med enumeratorn, bör en synkroniserad enumerator användas i stället för en normal enumerator så att traverseringen kan fortsätta från positionen precis efter den som har traverserats av det senaste MoveNext(). Dock, förutom fördelen att inget element hoppar över eller traverseras flera gånger, är nackdelen med den synkroniserade enumeratorn att prestandan blir något försämrad jämfört med en normal enumerator.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i raderna
            for (int i = 0; i < 5; i++)
            {
                Row row = worksheet.Cells.Rows[i];
                row[0].PutValue($"Row {i + 1}");
            }
            
            try
            {
                // Hämta RowCollection
                RowCollection rows = worksheet.Cells.Rows;
                
                // Anropa GetEnumerator med parametrar (reversed: true, sync: false)
                IEnumerator enumerator = rows.GetEnumerator(true, false);
                
                Console.WriteLine("Iterating rows in reverse order:");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
                
                // Anropa GetEnumerator med parametrar (reversed: false, sync: true)
                enumerator = rows.GetEnumerator(false, true);
                
                Console.WriteLine("\nIterating rows in normal order (synchronized):");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("RowCollectionGetEnumeratorDemo.xlsx");
        }
    }
}
```

### Se även

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


