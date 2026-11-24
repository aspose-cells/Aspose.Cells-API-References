---
title: "UnionRange.Intersect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Methode. Überschneidet einen anderen Bereich"
type: docs
url: /de/net/aspose.cells/unionrange/intersect/
---
## Intersect(string) {#intersect_2}

Schneidet einen anderen Bereich.

```csharp
public UnionRange Intersect(string range)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | String | Der Bereich. |

### Hinweise

Wenn die beiden Union-Bereiche nicht geschnitten werden, wird null zurückgegeben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodIntersectWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Beispieldaten einfügen
            worksheet.Cells["A1"].PutValue("A1");
            worksheet.Cells["B1"].PutValue("B1");
            worksheet.Cells["A2"].PutValue("A2");
            worksheet.Cells["B2"].PutValue("B2");

            // Erstelle einen UnionRange, der A1:B2 abdeckt
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            try
            {
                // Rufe Intersect mit einem Zeichenkettenparameter auf, der den Bereich A1:A2 darstellt
                UnionRange intersectionResult = unionRange.Intersect("A1:A2");

                // Zeige Informationen über die Schnittmenge an
                Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
                Console.WriteLine($"First row: {intersectionResult.FirstRow}");
                Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
                Console.WriteLine($"Row count: {intersectionResult.RowCount}");
                Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");

                // Markiere den Schnittbereich
                Style highlightStyle = workbook.CreateStyle();
                highlightStyle.BackgroundColor = System.Drawing.Color.LightGreen;
                intersectionResult.SetStyle(highlightStyle);

                Console.WriteLine("Intersect method executed successfully with parameter (String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Intersect method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("UnionRangeMethodIntersectWithStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Intersect(UnionRange) {#intersect_1}

Schneidet einen anderen Bereich.

```csharp
public UnionRange Intersect(UnionRange unionRange)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| unionRange | UnionRange | Der Bereich. |

### Hinweise

Wenn die beiden Union-Bereiche nicht geschnitten werden, wird null zurückgegeben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodIntersectWithUnionRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fülle einige Zellen mit Daten
            worksheet.Cells["A1"].PutValue("A1");
            worksheet.Cells["B1"].PutValue("B1");
            worksheet.Cells["C1"].PutValue("C1");
            worksheet.Cells["A2"].PutValue("A2");
            worksheet.Cells["B2"].PutValue("B2");
            worksheet.Cells["C2"].PutValue("C2");

            // Erstelle zwei Unionbereiche
            UnionRange range1 = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
            UnionRange range2 = worksheet.Cells.CreateRange("B1:C2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("B1:C2") });

            try
            {
                // Rufe die Intersect-Methode mit einem UnionRange-Parameter auf
                UnionRange intersectionResult = range1.Intersect(range2);

                // Zeige Informationen über die Schnittmenge an
                Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
                Console.WriteLine($"First row: {intersectionResult.FirstRow}");
                Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
                Console.WriteLine($"Row count: {intersectionResult.RowCount}");
                Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");

                // Markiere den Schnittbereich
                Style highlightStyle = workbook.CreateStyle();
                highlightStyle.BackgroundColor = System.Drawing.Color.Yellow;
                intersectionResult.SetStyle(highlightStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Intersect method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("UnionRangeMethodIntersectWithUnionRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Intersect(Range[]) {#intersect}

Schneidet einen anderen Bereich.

```csharp
public UnionRange Intersect(Range[] ranges)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereiche | Range[] | Der Bereich. |

### Hinweise

Wenn die beiden Union-Bereiche nicht geschnitten werden, wird null zurückgegeben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodIntersectWithRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten in Zellen erstellen
            worksheet.Cells["A1"].PutValue("A1");
            worksheet.Cells["B1"].PutValue("B1");
            worksheet.Cells["A2"].PutValue("A2");
            worksheet.Cells["B2"].PutValue("B2");

            // Erstelle Bereiche zum Schneiden
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B1");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A1:A2");
            Aspose.Cells.Range[] rangesToIntersect = new Aspose.Cells.Range[] { range1, range2 };

            // Hole den UnionRange des Arbeitsblatts
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            try
            {
                // Rufe die Intersect-Methode mit einem Range[]-Parameter auf
                UnionRange intersectionResult = unionRange.Intersect(rangesToIntersect);

                // Zeige Informationen über das Ergebnis der Schnittmenge an
                Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
                Console.WriteLine($"First row: {intersectionResult.FirstRow}");
                Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
                Console.WriteLine($"Row count: {intersectionResult.RowCount}");
                Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");

                // Markiere den Schnittbereich
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.Yellow;
                intersectionResult.SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Intersect method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("UnionRangeMethodIntersectWithRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


