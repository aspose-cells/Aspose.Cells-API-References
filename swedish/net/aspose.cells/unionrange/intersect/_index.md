---
title: "UnionRange.Intersect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange‑metod. Skär av ett annat område"
type: docs
url: /sv/net/aspose.cells/unionrange/intersect/
---
## Intersect(string) {#intersect_2}

Skär med ett annat område.

```csharp
public UnionRange Intersect(string range)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | String | Området. |

### Anmärkningar

Om de två unionområdena inte korsas, returneras null.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodIntersectWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite exempeldata
            worksheet.Cells["A1"].PutValue("A1");
            worksheet.Cells["B1"].PutValue("B1");
            worksheet.Cells["A2"].PutValue("A2");
            worksheet.Cells["B2"].PutValue("B2");

            // Skapa ett UnionRange som täcker A1:B2
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            try
            {
                // Anropa Intersect med en strängparameter som representerar området A1:A2
                UnionRange intersectionResult = unionRange.Intersect("A1:A2");

                // Visa information om korsningen
                Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
                Console.WriteLine($"First row: {intersectionResult.FirstRow}");
                Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
                Console.WriteLine($"Row count: {intersectionResult.RowCount}");
                Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");

                // Markera korsningsområdet
                Style highlightStyle = workbook.CreateStyle();
                highlightStyle.BackgroundColor = System.Drawing.Color.LightGreen;
                intersectionResult.SetStyle(highlightStyle);

                Console.WriteLine("Intersect method executed successfully with parameter (String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Intersect method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("UnionRangeMethodIntersectWithStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Intersect(UnionRange) {#intersect_1}

Skär med ett annat område.

```csharp
public UnionRange Intersect(UnionRange unionRange)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| unionRange | UnionRange | Området. |

### Anmärkningar

Om de två unionområdena inte korsas, returneras null.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodIntersectWithUnionRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i några data i celler
            worksheet.Cells["A1"].PutValue("A1");
            worksheet.Cells["B1"].PutValue("B1");
            worksheet.Cells["C1"].PutValue("C1");
            worksheet.Cells["A2"].PutValue("A2");
            worksheet.Cells["B2"].PutValue("B2");
            worksheet.Cells["C2"].PutValue("C2");

            // Skapa två unionområden
            UnionRange range1 = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
            UnionRange range2 = worksheet.Cells.CreateRange("B1:C2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("B1:C2") });

            try
            {
                // Anropa Intersect‑metoden med UnionRange‑parameter
                UnionRange intersectionResult = range1.Intersect(range2);

                // Visa information om korsningen
                Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
                Console.WriteLine($"First row: {intersectionResult.FirstRow}");
                Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
                Console.WriteLine($"Row count: {intersectionResult.RowCount}");
                Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");

                // Markera korsningsområdet
                Style highlightStyle = workbook.CreateStyle();
                highlightStyle.BackgroundColor = System.Drawing.Color.Yellow;
                intersectionResult.SetStyle(highlightStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Intersect method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("UnionRangeMethodIntersectWithUnionRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Intersect(Range[]) {#intersect}

Skär med ett annat område.

```csharp
public UnionRange Intersect(Range[] ranges)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ranges | Range[] | Området. |

### Anmärkningar

Om de två unionområdena inte korsas, returneras null.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodIntersectWithRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata i celler
            worksheet.Cells["A1"].PutValue("A1");
            worksheet.Cells["B1"].PutValue("B1");
            worksheet.Cells["A2"].PutValue("A2");
            worksheet.Cells["B2"].PutValue("B2");

            // Skapa områden att korsas
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B1");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A1:A2");
            Aspose.Cells.Range[] rangesToIntersect = new Aspose.Cells.Range[] { range1, range2 };

            // Hämta unionområdet för kalkylbladet
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            try
            {
                // Anropa Intersect‑metoden med Range[]‑parameter
                UnionRange intersectionResult = unionRange.Intersect(rangesToIntersect);

                // Visa information om resultatet av korsningen
                Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
                Console.WriteLine($"First row: {intersectionResult.FirstRow}");
                Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
                Console.WriteLine($"Row count: {intersectionResult.RowCount}");
                Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");

                // Markera korsningsområdet
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.Yellow;
                intersectionResult.SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Intersect method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("UnionRangeMethodIntersectWithRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


