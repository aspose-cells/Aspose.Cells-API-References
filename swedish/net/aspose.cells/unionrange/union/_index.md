---
title: "UnionRange.Union"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange‑metod. Unionera ett annat område"
type: docs
url: /sv/net/aspose.cells/unionrange/union/
---
## Union(string) {#union_2}

Förenar ett annat område.

```csharp
public UnionRange Union(string range)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | String | Området. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnionWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa initialt område och fyll i med data
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            range1[0, 0].PutValue("Range1");
            range1[0, 1].PutValue(100);
            range1[1, 0].PutValue("Data");
            range1[1, 1].PutValue(200);

            // Skapa UnionRange från det initiala området
            UnionRange unionRange = worksheet.Cells.CreateRange(range1.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range1 });

            try
            {
                // Anropa Union‑metoden med en strängparameter som representerar ett annat område
                UnionRange combinedRange = unionRange.Union("C1:D2");

                // Fyll i det andra intervallet med data
                worksheet.Cells["C1"].PutValue("Range2");
                worksheet.Cells["D1"].PutValue(300);
                worksheet.Cells["C2"].PutValue("More");
                worksheet.Cells["D2"].PutValue(400);

                Console.WriteLine("Union method executed successfully with parameter (String)");
                Console.WriteLine($"Combined range refers to: {combinedRange.RefersTo}");
                Console.WriteLine($"Total ranges in union: {combinedRange.RangeCount}");

                // Visa information om det kombinerade intervallet
                Console.WriteLine("\nCombined Range Info:");
                Console.WriteLine($"FirstRow: {combinedRange.FirstRow}, FirstColumn: {combinedRange.FirstColumn}");
                Console.WriteLine($"RowCount: {combinedRange.RowCount}, ColumnCount: {combinedRange.ColumnCount}");
                Console.WriteLine($"CellCount: {combinedRange.CellCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("UnionRangeMethodUnionWithStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Union(UnionRange) {#union_1}

Förenar ett annat område.

```csharp
public UnionRange Union(UnionRange unionRange)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| unionRange | UnionRange | Området. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnionWithUnionRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa det första intervallet och fyll det med data
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            range1[0, 0].PutValue("Range1");
            range1[0, 1].PutValue(100);
            range1[1, 0].PutValue("Data");
            range1[1, 1].PutValue(200);

            // Skapa det andra intervallet och fyll det med data
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C1:D2");
            range2[0, 0].PutValue("Range2");
            range2[0, 1].PutValue(300);
            range2[1, 0].PutValue("More");
            range2[1, 1].PutValue(400);

            // Skapa UnionRange från det första intervallet
            UnionRange unionRange1 = worksheet.Cells.CreateRange(range1.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range1 });

            // Skapa UnionRange från det andra intervallet
            UnionRange unionRange2 = worksheet.Cells.CreateRange(range2.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range2 });

            try
            {
                // Anropa Union-metoden med UnionRange-parameter
                UnionRange combinedRange = unionRange1.Union(unionRange2);

                Console.WriteLine("Union method executed successfully with parameter (UnionRange)");
                Console.WriteLine($"Combined range refers to: {combinedRange.RefersTo}");
                Console.WriteLine($"Total ranges in union: {combinedRange.RangeCount}");

                // Visa information om det kombinerade intervallet
                Console.WriteLine("\nCombined Range Info:");
                Console.WriteLine($"FirstRow: {combinedRange.FirstRow}, FirstColumn: {combinedRange.FirstColumn}");
                Console.WriteLine($"RowCount: {combinedRange.RowCount}, ColumnCount: {combinedRange.ColumnCount}");
                Console.WriteLine($"CellCount: {combinedRange.CellCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("UnionRangeMethodUnionWithUnionRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Union(Range[]) {#union}

Förenar områdena.

```csharp
public UnionRange Union(Range[] ranges)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ranges | Range[] | Intervallen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnionWithRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempelintervall för att demonstrera union
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("E5:F6");

            // Placera värden i intervallen för att visualisera dem
            range1[0, 0].PutValue("Range1");
            range2[0, 0].PutValue("Range2");
            range3[0, 0].PutValue("Range3");

            try
            {
                // Skapa initialt UnionRange
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range1 });

                // Anropa Union-metoden med Range[]-parameter
                Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range2, range3 };
                UnionRange resultUnion = unionRange.Union(rangesToUnion);

                Console.WriteLine("Union method executed successfully with parameters (Range[])");
                Console.WriteLine($"Resulting union range count: {resultUnion.RangeCount}");
                Console.WriteLine($"Resulting union refers to: {resultUnion.RefersTo}");

                // Markera unionsresultatet genom att sätta bakgrundsfärg
                Style highlightStyle = workbook.CreateStyle();
                highlightStyle.ForegroundColor = System.Drawing.Color.LightYellow;
                highlightStyle.Pattern = BackgroundType.Solid;
                resultUnion.SetStyle(highlightStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("UnionRangeMethodUnionWithRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


