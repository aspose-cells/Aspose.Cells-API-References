---
title: "AbstractFormulaChangeMonitor.OnFormatConditionFormulaChanged"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractFormulaChangeMonitor. El evento que se disparará cuando la fórmula de FormatCondition cambie"
type: docs
url: /es/net/aspose.cells/abstractformulachangemonitor/onformatconditionformulachanged/
---
## AbstractFormulaChangeMonitor.OnFormatConditionFormulaChanged method

El evento que se activará cuando la fórmula de FormatCondition cambie.

```csharp
public virtual void OnFormatConditionFormulaChanged(FormatCondition fc)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fc | FormatCondition | El objeto FormatCondition cuya fórmula se ha cambiado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractFormulaChangeMonitorMethodOnFormatConditionFormulaChangedWithFormatConditionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Crear un formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Crear condición de formato
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style = workbook.CreateStyle();
            fc.Style.Font.Color = System.Drawing.Color.Red;

            // Crear monitor personalizado
            var monitor = new CustomFormulaChangeMonitor();

            try
            {
                // Llamar al método OnFormatConditionFormulaChanged
                monitor.OnFormatConditionFormulaChanged(fc);

                Console.WriteLine("Method executed successfully with FormatCondition parameter");

                // Aplicar el formato condicional a un rango
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

### Ver también

* class [FormatCondition](../../formatcondition/)
* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


