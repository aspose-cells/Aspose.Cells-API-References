---
title: "AbstractFormulaChangeMonitor.OnFormatConditionFormulaChanged"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractFormulaChangeMonitor-metod. Händelsen som kommer att utlösas när formeln för FormatCondition ändras"
type: docs
url: /sv/net/aspose.cells/abstractformulachangemonitor/onformatconditionformulachanged/
---
## AbstractFormulaChangeMonitor.OnFormatConditionFormulaChanged method

Händelsen som utlöses när formeln för FormatCondition ändras.

```csharp
public virtual void OnFormatConditionFormulaChanged(FormatCondition fc)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fc | FormatCondition | FormatCondition-objektet vars formel har ändrats |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractFormulaChangeMonitorMethodOnFormatConditionFormulaChangedWithFormatConditionDemo
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

            // Skapa en villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Skapa formatvillkor
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style = workbook.CreateStyle();
            fc.Style.Font.Color = System.Drawing.Color.Red;

            // Skapa en anpassad övervakare
            var monitor = new CustomFormulaChangeMonitor();

            try
            {
                // Anropa metoden OnFormatConditionFormulaChanged
                monitor.OnFormatConditionFormulaChanged(fc);

                Console.WriteLine("Method executed successfully with FormatCondition parameter");

                // Tillämpa den villkorsstyrda formateringen på ett område
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 2;
                area.EndColumn = 0;
                fcs.AddArea(area);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OnFormatConditionFormulaChanged method: {ex.Message}");
            }

            workbook.Save("MethodOnFormatConditionFormulaChangedDemo.xlsx");
        }
    }

    public class CustomFormulaChangeMonitor : AbstractFormulaChangeMonitor
    {
        public override void OnFormatConditionFormulaChanged(FormatCondition fc)
        {
            Console.WriteLine($"Format condition formula changed. Type: {fc.Type}, Formula1: {fc.Formula1}, Formula2: {fc.Formula2}");
        }
    }

}
```

### Se även

* class [FormatCondition](../../formatcondition/)
* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


