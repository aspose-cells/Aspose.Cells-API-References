---
title: "AbstractFormulaChangeMonitor.OnFormatConditionFormulaChanged"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractFormulaChangeMonitor. L'evento che verrà attivato quando la formula di FormatCondition viene modificata"
type: docs
url: /it/net/aspose.cells/abstractformulachangemonitor/onformatconditionformulachanged/
---
## AbstractFormulaChangeMonitor.OnFormatConditionFormulaChanged method

L'evento che verrà attivato quando la formula di FormatCondition viene modificata.

```csharp
public virtual void OnFormatConditionFormulaChanged(FormatCondition fc)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fc | FormatCondition | L'oggetto FormatCondition la cui formula è modificata |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractFormulaChangeMonitorMethodOnFormatConditionFormulaChangedWithFormatConditionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Crea una formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Crea una condizione di formattazione
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style = workbook.CreateStyle();
            fc.Style.Font.Color = System.Drawing.Color.Red;

            // Crea un monitor personalizzato
            var monitor = new CustomFormulaChangeMonitor();

            try
            {
                // Chiama il metodo OnFormatConditionFormulaChanged
                monitor.OnFormatConditionFormulaChanged(fc);

                Console.WriteLine("Method executed successfully with FormatCondition parameter");

                // Applica la formattazione condizionale a un intervallo
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

### Vedi anche

* class [FormatCondition](../../formatcondition/)
* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


