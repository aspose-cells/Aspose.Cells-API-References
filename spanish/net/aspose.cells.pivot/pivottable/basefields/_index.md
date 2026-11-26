---
title: "PivotTable.BaseFields"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Devuelve todos los campos base de pivote en la PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/basefields/
---
## PivotTable.BaseFields property

Devuelve todos los campos base de pivote en la PivotTable.

```csharp
public PivotFieldCollection BaseFields { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyBaseFieldsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 5;

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Actualizar los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Acceder a la colección BaseFields
            PivotFieldCollection baseFields = pivotTable.BaseFields;
            
            // Mostrar los elementos originales de cada campo base
            Console.WriteLine("Base Fields and their Original Items:");
            foreach (PivotField field in baseFields)
            {
                Console.WriteLine($"Field: {field.Name}");
                string[] originalItems = field.OriginalItems;
                foreach (string item in originalItems)
                {
                    Console.WriteLine($"- {item}");
                }
            }
        }
    }
}
```

### Ver también

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


