---
title: "PivotItem.IsCalculatedItem"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotItem. Indica si este elemento dinámico es un elemento de fórmula calculada"
type: docs
url: /es/net/aspose.cells.pivot/pivotitem/iscalculateditem/
---
## PivotItem.IsCalculatedItem property

Indica si este elemento pivot es un elemento de fórmula calculada.

```csharp
public bool IsCalculatedItem { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsCalculatedItemDemo
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
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;
            worksheet.Cells["B5"].Value = 15;

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Calcular datos de tabla dinámica
            pivotTable.CalculateData();

            // Obtener el primer elemento dinámico del primer campo dinámico
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // Mostrar el valor de la propiedad IsCalculatedItem
            Console.WriteLine("IsCalculatedItem value: " + pivotItem.IsCalculatedItem);

            // Verificar si el elemento dinámico es un elemento calculado
            if (pivotItem.IsCalculatedItem)
            {
                Console.WriteLine("This pivot item is a calculated formula item.");
                Console.WriteLine("Formula: " + pivotItem.GetFormula());
            }
            else
            {
                Console.WriteLine("This pivot item is not a calculated formula item.");
            }

            // Guarda el libro de trabajo
            workbook.Save("PivotItemPropertyIsCalculatedItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


