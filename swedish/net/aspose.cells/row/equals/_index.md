---
title: "Row.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-metod. Kontrollerar om detta objekt refererar till samma rad som ett annat"
type: docs
url: /sv/net/aspose.cells/row/equals/
---
## Equals(object) {#equals_1}

Kontrollerar om detta objekt refererar till samma rad som ett annat.

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | Object | annat objekt |

### Returvärde

sant om två objekt refererar till samma rad.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa två rader för jämförelse
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];
            
            // Ställ in några egenskaper för att göra raderna olika
            row1.Height = 20;
            row2.Height = 25;
            
            try
            {
                // Anropa Equals-metoden med Object-parameter
                bool result1 = row1.Equals((object)row2);
                Console.WriteLine($"Comparing row1 with row2: {result1}");
                
                // Jämför row1 med sig själv
                bool result2 = row1.Equals((object)row1);
                Console.WriteLine($"Comparing row1 with itself: {result2}");
                
                // Jämför med null
                bool result3 = row1.Equals((object)null);
                Console.WriteLine($"Comparing row1 with null: {result3}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
            
            workbook.Save("RowMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Se även

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Row) {#equals}

Kontrollerar om detta objekt refererar till samma rad som ett annat radobjekt.

```csharp
public bool Equals(Row row)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Row | annat radobjekt |

### Returvärde

sant om två radobjekt refererar till samma rad.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två rader för jämförelse
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];

            // Ställ in några egenskaper för att göra raderna olika
            row1.Height = 20;
            row2.Height = 25;
            row1.IsHidden = false;
            row2.IsHidden = true;

            try
            {
                // Anropa Equals-metoden för att jämföra raderna
                bool areEqual = row1.Equals(row2);

                // Visa resultatet
                Console.WriteLine($"Are rows equal? {areEqual}");

                // Skapa ett annat radobjekt med samma egenskaper som row1
                Row row3 = worksheet.Cells.Rows[2];
                row3.Height = row1.Height;
                row3.IsHidden = row1.IsHidden;

                // Jämför row1 med row3 (bör vara lika)
                bool areEqual2 = row1.Equals(row3);
                Console.WriteLine($"Are rows equal after matching properties? {areEqual2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("RowEqualsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


