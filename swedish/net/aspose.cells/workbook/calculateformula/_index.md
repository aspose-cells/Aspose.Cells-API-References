---
title: "Workbook.CalculateFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Beräknar resultatet av formler"
type: docs
url: /sv/net/aspose.cells/workbook/calculateformula/
---
## CalculateFormula() {#calculateformula}

Beräknar resultatet av formler.

```csharp
public void CalculateFormula()
```

### Anmärkningar

För alla stödda formler, se listan på https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### Exempel

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
            
            // Ange värden och formler
            cells["A1"].PutValue(5);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=B1+10";
            
            // Beräkna formler
            workbook.CalculateFormula();
            
            // Visa resultat
            Console.WriteLine("A1 value: " + cells["A1"].IntValue);
            Console.WriteLine("B1 formula result: " + cells["B1"].IntValue);
            Console.WriteLine("C1 formula result: " + cells["C1"].IntValue);
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(bool) {#calculateformula_2}

Beräknar resultatet av formler.

```csharp
public void CalculateFormula(bool ignoreError)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ignoreError | Boolean | Anger om fel vid beräkning av formler ska döljas. Felet kan vara en funktion som inte stöds, externa länkar osv. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Åtkomst till det första kalkylbladet och dess celler
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Placera värden i den första raden (A1:E1)
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(i + 1); // Values 1-5
            }

            // Placera värden i den andra raden (A2:E2)
            for (int i = 0; i < 5; i++)
            {
                cells[1, i].PutValue((i + 1) * 10); // Values 10,20,30,40,50
            }

            // Ställ in en gemensam HLOOKUP-formel i den fjärde raden (A4:E4)
            cells[3, 0].SetSharedFormula("=HLOOKUP(A1,$A$1:$E$2,2,FALSE)", 1, 5);

            // Beräkna formler utan rekursiv beräkning
            wb.CalculateFormula(false);

            // Visa resultaten
            Console.WriteLine("Formula calculation results:");
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Cell {((char)('A' + i))}4 value: {cells[3, i].StringValue}");
            }
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(CalculationOptions) {#calculateformula_1}

Beräknar formler i den här arbetsboken.

```csharp
public void CalculateFormula(CalculationOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | CalculationOptions | Alternativ för beräkning |

### Exempel

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
            
            // Skapa en tabell och ange kolumnnamn
            sheet.Cells["A1"].PutValue("A");
            sheet.Cells["B1"].PutValue("B");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(2);
            
            // Ange formler och beräkna
            Cells cells = sheet.Cells;
            cells["C1"].PutValue("InvalidColumn");
            cells["D1"].Formula = "=INDIRECT(\"A\"&ROW())";
            cells["E1"].Formula = "=IFERROR(INDIRECT(\"B\"&ROW()),\"OK\")";
            
            // Beräkna formler med alternativ
            wb.CalculateFormula(new CalculationOptions());
            
            // Skriv ut resultat
            Console.WriteLine("D1 result: " + cells["D1"].StringValue);
            Console.WriteLine("E1 result: " + cells["E1"].StringValue);
        }
    }
}
```

### Se även

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


