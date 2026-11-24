---
title: "Row.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Methode. Prüft, ob dieses Objekt auf dieselbe Zeile wie ein anderes verweist"
type: docs
url: /de/net/aspose.cells/row/equals/
---
## Equals(object) {#equals_1}

Überprüft, ob dieses Objekt auf dieselbe Zeile wie ein anderes verweist.

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object | ein anderes Objekt |

### Rückgabewert

true, wenn zwei Objekte auf dieselbe Zeile verweisen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle zwei Zeilen zum Vergleich
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];
            
            // Setze einige Eigenschaften, um die Zeilen unterschiedlich zu machen
            row1.Height = 20;
            row2.Height = 25;
            
            try
            {
                // Rufe die Equals-Methode mit dem Object-Parameter auf
                bool result1 = row1.Equals((object)row2);
                Console.WriteLine($"Comparing row1 with row2: {result1}");
                
                // Vergleiche row1 mit sich selbst
                bool result2 = row1.Equals((object)row1);
                Console.WriteLine($"Comparing row1 with itself: {result2}");
                
                // Vergleiche mit null
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

### Siehe auch

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Row) {#equals}

Überprüft, ob dieses Objekt auf dieselbe Zeile wie ein anderes Zeilenobjekt verweist.

```csharp
public bool Equals(Row row)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Row | ein weiteres Zeilenobjekt |

### Rückgabewert

true, wenn zwei Zeilenobjekte auf dieselbe Zeile verweisen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle zwei Zeilen zum Vergleich
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];

            // Setze einige Eigenschaften, um die Zeilen unterschiedlich zu machen
            row1.Height = 20;
            row2.Height = 25;
            row1.IsHidden = false;
            row2.IsHidden = true;

            try
            {
                // Rufe die Equals-Methode auf, um die Zeilen zu vergleichen
                bool areEqual = row1.Equals(row2);

                // Ergebnis anzeigen
                Console.WriteLine($"Are rows equal? {areEqual}");

                // Erstelle eine weitere Zeile mit denselben Eigenschaften wie row1
                Row row3 = worksheet.Cells.Rows[2];
                row3.Height = row1.Height;
                row3.IsHidden = row1.IsHidden;

                // Vergleiche row1 mit row3 (sollte gleich sein)
                bool areEqual2 = row1.Equals(row3);
                Console.WriteLine($"Are rows equal after matching properties? {areEqual2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("RowEqualsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


