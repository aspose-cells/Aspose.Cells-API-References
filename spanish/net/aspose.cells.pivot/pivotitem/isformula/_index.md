---
title: "PivotItem.IsFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotItem. Indica si este elemento dinámico es un elemento de fórmula calculada"
type: docs
url: /es/net/aspose.cells.pivot/pivotitem/isformula/
---
## PivotItem.IsFormula property

Indica si este elemento pivot es un elemento de fórmula calculada.

```csharp
[Obsolete("Use PivotItem.IsCalculatedItem property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsFormula { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotItem.IsCalculatedItem. Esta propiedad será eliminada 12 meses después a partir de noviembre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Obtener el primer elemento dinámico
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // Mostrar el valor actual de IsFormula (propiedad obsoleta)
            Console.WriteLine("Current IsFormula value: " + pivotItem.IsFormula);

            // Establecer un nuevo valor para IsFormula (propiedad obsoleta)
            pivotItem.IsFormula = true;

            // Demostrar el efecto - esto marcaría el elemento dinámico como un elemento de fórmula
            Console.WriteLine("After setting IsFormula to true: " + pivotItem.IsFormula);

            // Nota: En el uso real, debe usar IsCalculatedItem en su lugar ya que IsFormula está obsoleto
            Console.WriteLine("IsCalculatedItem (recommended property): " + pivotItem.IsCalculatedItem);

            // Guardar el resultado
            workbook.Save("PivotItemPropertyIsFormulaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


