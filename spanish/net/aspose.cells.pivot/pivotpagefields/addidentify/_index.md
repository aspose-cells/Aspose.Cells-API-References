---
title: "PivotPageFields.AddIdentify"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotPageFields. Establece qué etiqueta de elemento en cada campo de página se usa para identificar el rango de datos. pageItemIndex.Length debe ser igual a PageFieldCount, así que por favor añada primero el campo de página."
type: docs
url: /es/net/aspose.cells.pivot/pivotpagefields/addidentify/
---
## PivotPageFields.AddIdentify method

Establece qué etiqueta de elemento en cada campo de página usar para identificar el rango de datos. pageItemIndex.Length debe ser igual a PageFieldCount, así que por favor agregue primero el campo de página.

```csharp
public void AddIdentify(int rangeIndex, int[] pageItemIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rangeIndex | Int32 | El índice del rango de datos de consolidación. |
| pageItemIndex | Int32[] | El índice del elemento de página en cada campo de página. pageItemIndex[2] = 1 significa que el segundo elemento en el tercer campo se usa para identificar este rango. pageItemIndex[1] = -1 significa que no hay elemento en el segundo campo para identificar este rango y MS creará automáticamente un elemento \"blank\" en el segundo campo para identificar este rango. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");
            worksheet.Cells["B4"].PutValue("C");

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Instanciar PivotPageFields directamente en lugar de acceder a través de PivotTable
            PivotPageFields pageFields = new PivotPageFields();

            try
            {
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                Console.WriteLine("AddIdentify executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


