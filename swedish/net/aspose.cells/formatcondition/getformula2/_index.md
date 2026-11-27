---
title: "FormatCondition.GetFormula2"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition method. Hämtar värdet eller uttrycket som är associerat med detta formatvillkor"
type: docs
url: /sv/net/aspose.cells/formatcondition/getformula2/
---
## GetFormula2(bool, bool) {#getformula2}

Hämtar värdet eller uttrycket som är kopplat till detta formatvillkor.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal)
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

    public class FormatConditionMethodGetFormula2WithBooleanBooleanDemo
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

            // Lägg till ett formatvillkor
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 0;
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");
            FormatCondition fc = fcs[conditionIndex];
            
            // Ange Formula2
            fc.Formula2 = "30";

            try
            {
                // Anropa GetFormula2 med (Boolean, Boolean)-parametrar
                string formula2 = fc.GetFormula2(false, false);
                
                // Visa resultatet
                Console.WriteLine("Formula2: " + formula2);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("FormatConditionMethodGetFormula2WithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Se även

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(bool, bool, int, int) {#getformula2_1}

Hämtar värdet eller uttrycket för cellens villkorliga formatering.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal, int row, int column)
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodGetFormula2WithBooleanBooleanInt32Int32Demo
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
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "=A3");
            FormatCondition fc = fcs[conditionIndex];

            try
            {
                // Anropa GetFormula2 med specifika parametrar (isR1C1, isLocal, rad, kolumn)
                string formula = fc.GetFormula2(false, false, 0, 0);
                
                Console.WriteLine("Formula2 retrieved successfully: " + formula);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean, Int32, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("FormatConditionMethodGetFormula2WithBooleanBooleanInt32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(int, int) {#getformula2_2}

Hämtar formeln för cellens villkorliga formatering.

```csharp
public string GetFormula2(int row, int column)
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

    public class FormatConditionMethodGetFormula2WithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            worksheet.Cells["A3"].PutValue(25);
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Lägg till villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 1;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "A1", "B3");

            // Hämta det första formatvillkoret
            FormatCondition fc = fcc[0];

            try
            {
                // Anropa GetFormula2 med specifika rad- och kolumnparametrar
                string formula = fc.GetFormula2(1, 0); // Row 1, Column 0 (A2)
                
                Console.WriteLine("Formula2 for cell (1,0): " + formula);
                Console.WriteLine("Method executed successfully with parameters (Int32, Int32)");

                // Tillämpa stil för att visualisera villkorsformateringen
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Red;
                fc.Style = style;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("FormatConditionMethodGetFormula2WithInt32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


