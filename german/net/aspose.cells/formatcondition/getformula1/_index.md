---
title: "FormatCondition.GetFormula1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Methode. Gibt den Wert oder Ausdruck zurück, der mit dieser Formatierungsbedingung verknüpft ist"
type: docs
url: /de/net/aspose.cells/formatcondition/getformula1/
---
## GetFormula1(bool, bool) {#getformula1}

Liest den Wert oder Ausdruck, der mit dieser Formatierungsbedingung verknüpft ist.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal)
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

    public class FormatConditionMethodGetFormula1WithBooleanBooleanDemo
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
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Holen Sie die erste Formatbedingung
            FormatCondition fc = fcc[0];

            try
            {
                // Rufen Sie GetFormula1 mit den Parametern (Boolean, Boolean) auf
                string formula = fc.GetFormula1(false, false);
                
                Console.WriteLine("Formula1: " + formula);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
                
                // Zeigen Sie die Wirkung, indem Sie den Bereich der bedingten Formatierung anzeigen
                Console.WriteLine($"Conditional format applied to range: A1:A3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("FormatConditionMethodGetFormula1WithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(bool, bool, int, int) {#getformula1_1}

Liest den Wert oder Ausdruck der bedingten Formatierung der Zelle.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal, int row, int column)
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

            // Füge eine Formatierungsbedingung hinzu
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[formatIndex];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 1, 0));
            int conditionIndex = fcc.AddCondition(FormatConditionType.Expression, OperatorType.None, "=IF(MOD(A1,2)=0,TRUE,FALSE)", null);

            // Holen Sie die Formel mit verschiedenen Parametern
            FormatCondition condition = fcc[conditionIndex];
            string formula1 = condition.GetFormula1(false, false, 0, 0);
            string formula2 = condition.GetFormula1(false, false, 1, 0);

            Console.WriteLine("Formula for row 0: " + formula1);
            Console.WriteLine("Formula for row 1: " + formula2);
        }
    }
}
```

### Siehe auch

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(int, int) {#getformula1_2}

Liest die Formel der bedingten Formatierung der Zelle.

```csharp
public string GetFormula1(int row, int column)
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

    public class FormatConditionMethodGetFormula1WithInt32Int32Demo
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

            // Bedingte Formatierung hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Holen Sie die erste Formatbedingung
            FormatCondition fc = fcc[0];

            try
            {
                // Rufen Sie GetFormula1 mit spezifischen Zeilen- und Spaltenparametern auf
                string formula = fc.GetFormula1(0, 0);
                
                Console.WriteLine("Formula1 for cell (0,0): " + formula);
                Console.WriteLine("Method executed successfully with parameters (Int32, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("FormatConditionMethodGetFormula1WithInt32Int32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


