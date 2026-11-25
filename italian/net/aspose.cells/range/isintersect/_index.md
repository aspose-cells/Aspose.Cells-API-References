---
title: "Range.IsIntersect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Indica se l'intervallo si interseca"
type: docs
url: /it/net/aspose.cells/range/isintersect/
---
## Range.IsIntersect method

Indica se l'intervallo è intersecato.

```csharp
public bool IsIntersect(Range range)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | Intervallo | L'intervallo. |

### Valore di ritorno

Se l'intervallo si interseca.

### Osservazioni

Se i due intervalli non si trovano nello stesso foglio di lavoro, restituisce false.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodIsIntersectWithRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due intervalli per testare l'intersezione
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B3:D8");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("C10:D15");

            try
            {
                // Verifica se range1 si interseca con range2 (dovrebbe intersecarsi)
                bool result1 = range1.IsIntersect(range2);
                Console.WriteLine($"Range A1:B5 intersects with B3:D8: {result1}");

                // Verifica se range1 si interseca con range3 (non dovrebbe intersecarsi)
                bool result2 = range1.IsIntersect(range3);
                Console.WriteLine($"Range A1:B5 intersects with C10:D15: {result2}");

                // Riempi gli intervalli con colori diversi per visualizzarli
                Style style1 = workbook.CreateStyle();
                style1.ForegroundColor = System.Drawing.Color.LightBlue;
                style1.Pattern = BackgroundType.Solid;
                range1.SetStyle(style1);

                Style style2 = workbook.CreateStyle();
                style2.ForegroundColor = System.Drawing.Color.LightGreen;
                style2.Pattern = BackgroundType.Solid;
                range2.SetStyle(style2);

                Style style3 = workbook.CreateStyle();
                style3.ForegroundColor = System.Drawing.Color.LightPink;
                style3.Pattern = BackgroundType.Solid;
                range3.SetStyle(style3);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsIntersect method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("RangeMethodIsIntersectWithRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


