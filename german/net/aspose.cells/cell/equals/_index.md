---
title: "Cell.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Prüft, ob dieses Objekt auf dieselbe Zelle wie ein anderes verweist"
type: docs
url: /de/net/aspose.cells/cell/equals/
---
## Equals(object) {#equals_1}

Prüft, ob dieses Objekt auf dieselbe Zelle wie ein anderes verweist.

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object | ein anderes Objekt |

### Rückgabewert

wahr, wenn zwei Objekte auf dieselbe Zelle verweisen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zellen von verschiedenen Positionen aus zugreifen
            Cell cellA1 = worksheet.Cells["A1"];
            Cell anotherCellA1 = worksheet.Cells[0, 0]; // Same physical cell as A1
            Cell cellB1 = worksheet.Cells["B1"];

            // Identische Werte in verschiedenen Zellen setzen
            cellA1.PutValue("Aspose.Cells");
            cellB1.PutValue("Aspose.Cells");

            try
            {
                // Gleiche physische Zellreferenzen vergleichen
                bool sameCellComparison = cellA1.Equals(anotherCellA1);
                Console.WriteLine($"Same cell comparison: {sameCellComparison}"); // True

                // Verschiedene Zellen mit identischem Inhalt vergleichen
                bool differentCellComparison = cellA1.Equals(cellB1);
                Console.WriteLine($"Different cell comparison: {differentCellComparison}"); // False

                // Zelle mit Nicht-Zell-Objekt vergleichen
                bool invalidTypeComparison = cellA1.Equals("Aspose.Cells");
                Console.WriteLine($"Invalid type comparison: {invalidTypeComparison}"); // False
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("CellMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Cell) {#equals}

Prüft, ob dieses Objekt auf dieselbe Zelle wie ein anderes Zellenobjekt verweist.

```csharp
public bool Equals(Cell cell)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zelle | Zelle | ein anderes Zellenobjekt |

### Rückgabewert

wahr, wenn zwei Zellenobjekte auf dieselbe Zelle verweisen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithCellDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zellen an verschiedenen Positionen erstellen (A1 und B1)
            Cell cellA1 = worksheet.Cells[0, 0];
            Cell cellB1 = worksheet.Cells[0, 1];

            // Identische Werte in beiden Zellen setzen
            cellA1.Value = "Aspose.Cells Comparison";
            cellB1.Value = "Aspose.Cells Comparison";

            try
            {
                // cellA1 mit cellB1 vergleichen (verschiedene Positionen)
                bool equalsResult = cellA1.Equals(cellB1);
                Console.WriteLine($"Cell A1 equals Cell B1: {equalsResult}");

                // cellA1 mit sich selbst vergleichen (gleiche Instanz)
                equalsResult = cellA1.Equals(cellA1);
                Console.WriteLine($"Cell A1 equals itself: {equalsResult}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("CellMethodEqualsWithCellDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


