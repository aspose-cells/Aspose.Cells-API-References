---
title: "FormatCondition.GetFormula1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition method. Hämtar värdet eller uttrycket som är associerat med detta formatvillkor"
type: docs
url: /sv/net/aspose.cells/formatcondition/getformula1/
---
## GetFormula1(bool, bool) {#getformula1}

Hämtar värdet eller uttrycket som är kopplat till detta formatvillkor.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | Boolean | Om formeln behöver formateras som R1C1. |
| isLocal | Boolean | Om formeln behöver formateras enligt lokala inställningar. |

### Returvärde

Värdet eller uttrycket som är associerat med detta formatvillkor.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodGetFormula1WithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Lägg till ett villkorsformat
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Hämta det första formatvillkoret
            FormatCondition fc = fcc[0];

            try
            {
                // Anropa GetFormula1 med parametrar (Boolean, Boolean)
                string formula = fc.GetFormula1(false, false);
                
                Console.WriteLine("Formula1: " + formula);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
                
                // Visa effekten genom att visa det villkorsformaterade området
                Console.WriteLine($"Conditional format applied to range: A1:A3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("FormatConditionMethodGetFormula1WithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Se även

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(bool, bool, int, int) {#getformula1_1}

Hämtar värdet eller uttrycket för cellens villkorliga formatering.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal, int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | Boolean | Om formeln behöver formateras som R1C1. |
| isLocal | Boolean | Om formeln behöver formateras enligt lokala inställningar. |
| row | Int32 | Radindexet. |
| column | Int32 | Kolumnindexet. |

### Returvärde

Värdet eller uttrycket som är kopplat till cellens villkorsformatering.

### Anmärkningar

Den angivna cellen måste ingå i denna villkorsformatering, annars returneras null.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionMethodGetFormula1WithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett formatvillkor
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[formatIndex];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 1, 0));
            int conditionIndex = fcc.AddCondition(FormatConditionType.Expression, OperatorType.None, "=IF(MOD(A1,2)=0,TRUE,FALSE)", null);

            // Hämta formeln med olika parametrar
            FormatCondition condition = fcc[conditionIndex];
            string formula1 = condition.GetFormula1(false, false, 0, 0);
            string formula2 = condition.GetFormula1(false, false, 1, 0);

            Console.WriteLine("Formula for row 0: " + formula1);
            Console.WriteLine("Formula for row 1: " + formula2);
        }
    }
}
```

### Se även

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(int, int) {#getformula1_2}

Hämtar formeln för cellens villkorliga formatering.

```csharp
public string GetFormula1(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |
| column | Int32 | Kolumnindexet. |

### Returvärde

Formeln.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodGetFormula1WithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Lägg till villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Hämta det första formatvillkoret
            FormatCondition fc = fcc[0];

            try
            {
                // Anropa GetFormula1 med specifika rad- och kolumnparametrar
                string formula = fc.GetFormula1(0, 0);
                
                Console.WriteLine("Formula1 for cell (0,0): " + formula);
                Console.WriteLine("Method executed successfully with parameters (Int32, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("FormatConditionMethodGetFormula1WithInt32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


