---
title: "UnionRange.Union"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Methode. Vereinigt einen anderen Bereich"
type: docs
url: /de/net/aspose.cells/unionrange/union/
---
## Union(string) {#union_2}

Vereint einen anderen Bereich.

```csharp
public UnionRange Union(string range)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | String | Der Bereich. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnionWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie den Anfangsbereich und füllen Sie ihn mit Daten
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            range1[0, 0].PutValue("Range1");
            range1[0, 1].PutValue(100);
            range1[1, 0].PutValue("Data");
            range1[1, 1].PutValue(200);

            // Erstellen Sie UnionRange aus dem Anfangsbereich
            UnionRange unionRange = worksheet.Cells.CreateRange(range1.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range1 });

            try
            {
                // Rufen Sie die Union-Methode mit einem Zeichenkettenparameter auf, der einen anderen Bereich darstellt
                UnionRange combinedRange = unionRange.Union("C1:D2");

                // Füllen Sie den zweiten Bereich mit Daten
                worksheet.Cells["C1"].PutValue("Range2");
                worksheet.Cells["D1"].PutValue(300);
                worksheet.Cells["C2"].PutValue("More");
                worksheet.Cells["D2"].PutValue(400);

                Console.WriteLine("Union method executed successfully with parameter (String)");
                Console.WriteLine($"Combined range refers to: {combinedRange.RefersTo}");
                Console.WriteLine($"Total ranges in union: {combinedRange.RangeCount}");

                // Zeigen Sie Informationen über den kombinierten Bereich an
                Console.WriteLine("\nCombined Range Info:");
                Console.WriteLine($"FirstRow: {combinedRange.FirstRow}, FirstColumn: {combinedRange.FirstColumn}");
                Console.WriteLine($"RowCount: {combinedRange.RowCount}, ColumnCount: {combinedRange.ColumnCount}");
                Console.WriteLine($"CellCount: {combinedRange.CellCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("UnionRangeMethodUnionWithStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Union(UnionRange) {#union_1}

Vereint einen anderen Bereich.

```csharp
public UnionRange Union(UnionRange unionRange)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| unionRange | UnionRange | Der Bereich. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnionWithUnionRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle den ersten Bereich und fülle ihn mit Daten
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            range1[0, 0].PutValue("Range1");
            range1[0, 1].PutValue(100);
            range1[1, 0].PutValue("Data");
            range1[1, 1].PutValue(200);

            // Erstelle den zweiten Bereich und fülle ihn mit Daten
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C1:D2");
            range2[0, 0].PutValue("Range2");
            range2[0, 1].PutValue(300);
            range2[1, 0].PutValue("More");
            range2[1, 1].PutValue(400);

            // Erstelle ein UnionRange aus dem ersten Bereich
            UnionRange unionRange1 = worksheet.Cells.CreateRange(range1.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range1 });

            // Erstelle ein UnionRange aus dem zweiten Bereich
            UnionRange unionRange2 = worksheet.Cells.CreateRange(range2.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range2 });

            try
            {
                // Rufe die Union-Methode mit dem UnionRange-Parameter auf
                UnionRange combinedRange = unionRange1.Union(unionRange2);

                Console.WriteLine("Union method executed successfully with parameter (UnionRange)");
                Console.WriteLine($"Combined range refers to: {combinedRange.RefersTo}");
                Console.WriteLine($"Total ranges in union: {combinedRange.RangeCount}");

                // Zeigen Sie Informationen über den kombinierten Bereich an
                Console.WriteLine("\nCombined Range Info:");
                Console.WriteLine($"FirstRow: {combinedRange.FirstRow}, FirstColumn: {combinedRange.FirstColumn}");
                Console.WriteLine($"RowCount: {combinedRange.RowCount}, ColumnCount: {combinedRange.ColumnCount}");
                Console.WriteLine($"CellCount: {combinedRange.CellCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("UnionRangeMethodUnionWithUnionRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Union(Range[]) {#union}

Vereint die Bereiche.

```csharp
public UnionRange Union(Range[] ranges)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereiche | Range[] | Die Bereiche. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnionWithRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle Beispielbereiche, um die Vereinigung zu demonstrieren
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("E5:F6");

            // Setze Werte in die Bereiche, um sie zu visualisieren
            range1[0, 0].PutValue("Range1");
            range2[0, 0].PutValue("Range2");
            range3[0, 0].PutValue("Range3");

            try
            {
                // Erstelle den initialen Union-Bereich
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range1 });

                // Rufe die Union-Methode mit dem Range[]-Parameter auf
                Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range2, range3 };
                UnionRange resultUnion = unionRange.Union(rangesToUnion);

                Console.WriteLine("Union method executed successfully with parameters (Range[])");
                Console.WriteLine($"Resulting union range count: {resultUnion.RangeCount}");
                Console.WriteLine($"Resulting union refers to: {resultUnion.RefersTo}");

                // Markiere das Unionsergebnis, indem du die Hintergrundfarbe festlegst
                Style highlightStyle = workbook.CreateStyle();
                highlightStyle.ForegroundColor = System.Drawing.Color.LightYellow;
                highlightStyle.Pattern = BackgroundType.Solid;
                resultUnion.SetStyle(highlightStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("UnionRangeMethodUnionWithRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


