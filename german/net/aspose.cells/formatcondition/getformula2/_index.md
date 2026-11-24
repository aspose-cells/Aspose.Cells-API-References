---
title: "FormatCondition.GetFormula2"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Methode. Gibt den Wert oder Ausdruck zurück, der mit dieser Formatierungsbedingung verknüpft ist"
type: docs
url: /de/net/aspose.cells/formatcondition/getformula2/
---
## GetFormula2(bool, bool) {#getformula2}

Liest den Wert oder Ausdruck, der mit dieser Formatierungsbedingung verknüpft ist.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | Boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | Boolean | Ob die Formel nach den Ländereinstellungen formatiert werden muss. |

### Rückgabewert

Der Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodGetFormula2WithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Füge eine Formatierungsbedingung hinzu
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 0;
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");
            FormatCondition fc = fcs[conditionIndex];
            
            // Setzen Sie Formula2
            fc.Formula2 = "30";

            try
            {
                // Rufen Sie GetFormula2 mit den Parametern (Boolean, Boolean) auf
                string formula2 = fc.GetFormula2(false, false);
                
                // Ergebnis anzeigen
                Console.WriteLine("Formula2: " + formula2);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("FormatConditionMethodGetFormula2WithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(bool, bool, int, int) {#getformula2_1}

Liest den Wert oder Ausdruck der bedingten Formatierung der Zelle.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal, int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | Boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | Boolean | Ob die Formel nach den Ländereinstellungen formatiert werden muss. |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |

### Rückgabewert

Der Wert oder Ausdruck, der mit der bedingten Formatierung der Zelle verknüpft ist.

### Hinweise

Die angegebene Zelle muss von dieser bedingten Formatierung enthalten sein, sonst wird null zurückgegeben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodGetFormula2WithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Fügen Sie ein bedingtes Format hinzu
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "=A3");
            FormatCondition fc = fcs[conditionIndex];

            try
            {
                // Rufen Sie GetFormula2 mit bestimmten Parametern (isR1C1, isLocal, Zeile, Spalte) auf
                string formula = fc.GetFormula2(false, false, 0, 0);
                
                Console.WriteLine("Formula2 retrieved successfully: " + formula);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean, Int32, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("FormatConditionMethodGetFormula2WithBooleanBooleanInt32Int32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(int, int) {#getformula2_2}

Liest die Formel der bedingten Formatierung der Zelle.

```csharp
public string GetFormula2(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |

### Rückgabewert

Die Formel.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodGetFormula2WithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            worksheet.Cells["A3"].PutValue(25);
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Bedingte Formatierung hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 1;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "A1", "B3");

            // Holen Sie die erste Formatbedingung
            FormatCondition fc = fcc[0];

            try
            {
                // Rufen Sie GetFormula2 mit spezifischen Zeilen- und Spaltenparametern auf
                string formula = fc.GetFormula2(1, 0); // Row 1, Column 0 (A2)
                
                Console.WriteLine("Formula2 for cell (1,0): " + formula);
                Console.WriteLine("Method executed successfully with parameters (Int32, Int32)");

                // Wenden Sie einen Stil an, um die bedingte Formatierung zu visualisieren
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Red;
                fc.Style = style;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("FormatConditionMethodGetFormula2WithInt32Int32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


