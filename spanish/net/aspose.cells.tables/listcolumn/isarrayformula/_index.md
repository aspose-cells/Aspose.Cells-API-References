---
title: "ListColumn.IsArrayFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListColumn. Indica si la fórmula es una fórmula de matriz"
type: docs
url: /es/net/aspose.cells.tables/listcolumn/isarrayformula/
---
## ListColumn.IsArrayFormula property

Indica si la fórmula es una fórmula de matriz.

```csharp
public bool IsArrayFormula { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnPropertyIsArrayFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para crear una tabla
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(20);

            // Crear un objeto tabla/lista
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[tableIndex];

            // Agregar una fórmula de matriz a la segunda columna
            listObject.ListColumns[1].Formula = "{=SUM(A2:A3*B2:B3)}";

            try
            {
                // Acceder a la propiedad IsArrayFormula (solo lectura)
                bool isArrayFormula = listObject.ListColumns[1].IsArrayFormula;

                // Mostrar el valor
                Console.WriteLine("IsArrayFormula value: " + isArrayFormula);

                // Guarda el libro de trabajo
                workbook.Save("IsArrayFormulaDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


