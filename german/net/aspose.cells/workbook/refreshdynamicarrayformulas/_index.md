---
title: "Workbook.RefreshDynamicArrayFormulas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Aktualisiert den Spill von dynamischen Array-Formeln in einen neuen Bereich benachbarter Zellen basierend auf den aktuellen Daten. Andere Formeln in der Arbeitsmappe werden nicht rekursiv berechnet, selbst wenn sie von dynamischen Array-Formeln verwendet wurden."
type: docs
url: /de/net/aspose.cells/workbook/refreshdynamicarrayformulas/
---
## RefreshDynamicArrayFormulas(bool) {#refreshdynamicarrayformulas}

Aktualisiert dynamische Array‑Formeln (erweitern sich in einen neuen Bereich benachbarter Zellen gemäß den aktuellen Daten). Andere Formeln in der Arbeitsmappe werden nicht rekursiv berechnet, selbst wenn sie von dynamischen Array‑Formeln verwendet werden.

```csharp
public void RefreshDynamicArrayFormulas(bool calculate)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| berechnen | Boolean | Ob die Werte für diese dynamischen Array-Formeln berechnet und aktualisiert werden |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet1 = wb.Worksheets[0];
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");

            // Initiale Daten und dynamische Array-Formeln einrichten
            sheet1.Cells["A1"].PutValue("B1:B3");
            sheet1.Cells["A2"].SetDynamicArrayFormula("=INDIRECT(A1)", new FormulaParseOptions(), true);
            sheet2.Cells["B1"].SetDynamicArrayFormula("=TRANSPOSE(Sheet1!A2#)", new FormulaParseOptions(), true);

            Console.WriteLine("Before refresh:");
            PrintSpillStatus(sheet1, sheet2);

            // Den Bereich ändern und Formeln aktualisieren
            sheet1.Cells["A1"].PutValue("B1:B5");
            wb.RefreshDynamicArrayFormulas(true);

            Console.WriteLine("\nAfter refresh:");
            PrintSpillStatus(sheet1, sheet2);
        }

        private static void PrintSpillStatus(Worksheet sheet1, Worksheet sheet2)
        {
            Console.WriteLine("Sheet1 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet1.Cells.CheckCell(i, 0);
                Console.WriteLine($"Row {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
            }

            Console.WriteLine("\nSheet2 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet2.Cells.CheckCell(0, i);
                Console.WriteLine($"Column {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
            }
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshDynamicArrayFormulas(bool, CalculationOptions) {#refreshdynamicarrayformulas_1}

Aktualisiert dynamische Array‑Formeln (erweitern sich in einen neuen Bereich benachbarter Zellen gemäß den aktuellen Daten).

```csharp
public void RefreshDynamicArrayFormulas(bool calculate, CalculationOptions copts)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| berechnen | Boolean | Ob die Werte für diese dynamischen Array-Formeln berechnet und aktualisiert werden |
| copts | CalculationOptions | Die Optionen zur Berechnung von Formeln |

### Hinweise

Aus Performance‑Gründen aktualisieren wir nicht automatisch alle dynamischen Array-Formeln, wenn sich die Formel selbst oder die referenzierten Daten ändern. Daher muss der Benutzer diese Methode manuell aufrufen, nachdem Vorgänge durchgeführt wurden, die dynamische Array-Formeln beeinflussen können, z. B. das Importieren/Setzen von Zellwerten, Einfügen/Löschen von Zeilen/Spalten/Bereichen usw. Für die meisten Formeln mit Funktionen muss zur Berechnung des Spill‑Bereichs auch die Formel berechnet werden, sodass im Allgemeinen der Wert "true" für das Flag "calculate" bevorzugt wird. Ist die Formel einfach, etwa ein Bereichsverweis oder ein Array (z. B. "=C1:E5", "={1,2;3,4}", …), eine einfache Funktion auf einem Bereich oder Array (z. B. "=ABS(C1:E5)", "=1+{1,2;3,4}", …) und werden alle Formeln später berechnet (z. B. durch [`CalculateFormula`](../calculateformula/)), kann die Verwendung des Werts "false" für das Flag "calculate" die doppelte Berechnung vermeiden und die Performance verbessern.

### Beispiele

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanCalculationOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispielhafte dynamische Array-Formel hinzufügen
            worksheet.Cells["A1"].Formula = "=SEQUENCE(5)";
            
            // Berechnungsoptionen erstellen
            CalculationOptions opts = new CalculationOptions();
            opts.CalcStackSize = 100;
            
            // Dynamische Array-Formeln mit Berechnungsoptionen aktualisieren
            workbook.RefreshDynamicArrayFormulas(true, opts);
            
            // Arbeitsmappen-Formeln berechnen
            workbook.CalculateFormula(opts);
            
            // Ergebnis von A1:A5 ausgeben
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].Value);
            }
        }
    }
}
```

### Siehe auch

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


