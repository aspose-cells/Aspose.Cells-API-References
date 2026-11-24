---
title: "Workbook.CalculateFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Berechnet das Ergebnis von Formeln"
type: docs
url: /de/net/aspose.cells/workbook/calculateformula/
---
## CalculateFormula() {#calculateformula}

Berechnet das Ergebnis von Formeln.

```csharp
public void CalculateFormula()
```

### Hinweise

Für alle unterstützten Formeln siehe bitte die Liste unter https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Werte und Formeln festlegen
            cells["A1"].PutValue(5);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=B1+10";
            
            // Formeln berechnen
            workbook.CalculateFormula();
            
            // Ergebnisse anzeigen
            Console.WriteLine("A1 value: " + cells["A1"].IntValue);
            Console.WriteLine("B1 formula result: " + cells["B1"].IntValue);
            Console.WriteLine("C1 formula result: " + cells["C1"].IntValue);
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(bool) {#calculateformula_2}

Berechnet das Ergebnis von Formeln.

```csharp
public void CalculateFormula(bool ignoreError)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ignoreError | Boolean | Gibt an, ob Fehler bei der Berechnung von Formeln ausgeblendet werden sollen. Der Fehler kann eine nicht unterstützte Funktion, externe Links usw. sein. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Auf das erste Arbeitsblatt und seine Zellen zugreifen
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Werte in die erste Zeile einfügen (A1:E1)
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(i + 1); // Values 1-5
            }

            // Werte in die zweite Zeile einfügen (A2:E2)
            for (int i = 0; i < 5; i++)
            {
                cells[1, i].PutValue((i + 1) * 10); // Values 10,20,30,40,50
            }

            // Gemeinsame HLOOKUP-Formel in der vierten Zeile festlegen (A4:E4)
            cells[3, 0].SetSharedFormula("=HLOOKUP(A1,$A$1:$E$2,2,FALSE)", 1, 5);

            // Formeln ohne rekursive Berechnung berechnen
            wb.CalculateFormula(false);

            // Ergebnisse anzeigen
            Console.WriteLine("Formula calculation results:");
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Cell {((char)('A' + i))}4 value: {cells[3, i].StringValue}");
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

## CalculateFormula(CalculationOptions) {#calculateformula_1}

Formeln in dieser Arbeitsmappe werden berechnet.

```csharp
public void CalculateFormula(CalculationOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | CalculationOptions | Optionen für die Berechnung |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaWithCalculationOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Eine Tabelle erstellen und Spaltennamen festlegen
            sheet.Cells["A1"].PutValue("A");
            sheet.Cells["B1"].PutValue("B");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(2);
            
            // Formeln festlegen und berechnen
            Cells cells = sheet.Cells;
            cells["C1"].PutValue("InvalidColumn");
            cells["D1"].Formula = "=INDIRECT(\"A\"&ROW())";
            cells["E1"].Formula = "=IFERROR(INDIRECT(\"B\"&ROW()),\"OK\")";
            
            // Formeln mit Optionen berechnen
            wb.CalculateFormula(new CalculationOptions());
            
            // Ergebnisse ausgeben
            Console.WriteLine("D1 result: " + cells["D1"].StringValue);
            Console.WriteLine("E1 result: " + cells["E1"].StringValue);
        }
    }
}
```

### Siehe auch

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


