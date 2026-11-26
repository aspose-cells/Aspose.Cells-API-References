---
title: "PivotConditionalFormat.RuleType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotConditionalFormat. Obtener y establecer el tipo de regla para el formato condicional de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivotconditionalformat/ruletype/
---
## PivotConditionalFormat.RuleType property

Obtener y establecer el tipo de regla para el formato condicional de la tabla dinámica.

```csharp
public PivotConditionFormatRuleType RuleType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotConditionalFormatPropertyRuleTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crear datos mínimos para la tabla dinámica
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "Value";

                // Crear tabla dinámica
                int pivotIndex = worksheet.PivotTables.Add("A1:A2", "C3", "DemoPivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Agregar formato condicional
                int formatIndex = pivotTable.ConditionalFormats.Add();
                PivotConditionalFormat format = pivotTable.ConditionalFormats[formatIndex];

                // Demostrar la propiedad RuleType
                Console.WriteLine("Initial RuleType: " + format.RuleType);
                
                // Establecer nuevo tipo de regla
                format.RuleType = PivotConditionFormatRuleType.Row;
                Console.WriteLine("Updated RuleType: " + format.RuleType);

                workbook.Save("RuleTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [PivotConditionFormatRuleType](../../pivotconditionformatruletype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


