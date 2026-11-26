---
title: "PivotItem.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotItem. Obtiene el valor del elemento de pivote"
type: docs
url: /es/net/aspose.cells.pivot/pivotitem/value/
---
## PivotItem.Value property

Obtiene el valor del elemento pivot

```csharp
public object Value { get; }
```

### Ejemplos

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyValueDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Obtener el campo de pivote
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Procesar elementos de pivote
            List<string> valuesToShow = new List<string> { "Apple", "Banana" };
            
            Console.WriteLine("Pivot Items Before Filtering:");
            PrintPivotItems(pivotField);

            // Filtrar elementos de pivote basándose en la propiedad Value
            for (int i = 0; i < pivotField.PivotItems.Count; i++)
            {
                PivotItem item = pivotField.PivotItems[i];
                string itemValue = item.Value?.ToString() ?? "";
                
                if (!valuesToShow.Contains(itemValue))
                {
                    item.IsHidden = true;
                }
            }

            Console.WriteLine("\nPivot Items After Filtering:");
            PrintPivotItems(pivotField);
        }

        private static void PrintPivotItems(PivotField pivotField)
        {
            for (int i = 0; i < pivotField.PivotItems.Count; i++)
            {
                PivotItem item = pivotField.PivotItems[i];
                Console.WriteLine($"Name: {item.Name}, Value: {item.Value}, Hidden: {item.IsHidden}");
            }
        }
    }
}
```

### Ver también

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


