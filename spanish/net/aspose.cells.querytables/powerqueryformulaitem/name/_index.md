---
title: "PowerQueryFormulaItem.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PowerQueryFormulaItem. Obtiene el nombre del elemento"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformulaitem/name/
---
## PowerQueryFormulaItem.Name property

Obtiene el nombre del elemento.

```csharp
public string Name { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaItemPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de Power Query de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            
            // Guardar para activar la creación de Power Query
            string sourcePath = "pq_source.xlsx";
            workbook.Save(sourcePath);
            
            // Reabrir para acceder a las fórmulas de Power Query
            workbook = new Workbook(sourcePath);
            Aspose.Cells.QueryTables.DataMashup mashupData = workbook.DataMashup;
            
            // Procesar fórmulas de Power Query
            foreach (Aspose.Cells.QueryTables.PowerQueryFormula formula in mashupData.PowerQueryFormulas)
            {
                Console.WriteLine("Formula Name: " + formula.Name);
                
                foreach (Aspose.Cells.QueryTables.PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                {
                    Console.WriteLine("  Item Name: " + item.Name);
                    
                    // Demostrar el uso de la propiedad Name
                    if (item.Name == "Source")
                    {
                        Console.WriteLine("Original Value: " + item.Value);
                        item.Value = "ModifiedSource";
                        Console.WriteLine("Modified Value: " + item.Value);
                    }
                }
            }
            
            // Guardar el libro de trabajo modificado
            workbook.Save("pq_modified.xlsx");
        }
    }
}
```

### Ver también

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


