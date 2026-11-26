---
title: "PivotField.GetCalculatedFieldFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "PivotField method. Obtén la cadena de fórmula del campo calculado especificado"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/getcalculatedfieldformula/
---
## PivotField.GetCalculatedFieldFormula method

Obtén la cadena de fórmula del campo calculado especificado.

```csharp
[Obsolete("Use PivotField.GetFormula() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string GetCalculatedFieldFormula()
```

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método PivotField.GetFormula(). Este método será eliminado 12 meses después, a partir de agosto de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGetCalculatedFieldFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;
            worksheet.Cells["C1"].Value = "Profit";
            worksheet.Cells["C2"].Value = 20;
            worksheet.Cells["C3"].Value = 30;
            worksheet.Cells["C4"].Value = 25;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Profit");

            // Agregar un campo calculado usando la PivotFieldCollection
            PivotFieldCollection pivotFields = pivotTable.DataFields;
            pivotTable.AddCalculatedField("ProfitMargin", "Profit/Sales", true);

            try
            {
                // Obtener el campo calculado de DataFields
                PivotField calculatedField = pivotTable.DataFields[2]; // Index 2 for the calculated field

                // Verificar si es un campo calculado
                if (calculatedField.IsCalculatedField)
                {
                    // Obtener la fórmula del campo calculado
                    string formula = calculatedField.GetFormula();
                    Console.WriteLine($"Calculated field formula: {formula}");

                    // Guarda el libro de trabajo
                    workbook.Save("GetCalculatedFieldFormulaDemo.xlsx");
                    Console.WriteLine("Workbook saved successfully.");
                }
                else
                {
                    Console.WriteLine("The field is not a calculated field.");
                }
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

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


