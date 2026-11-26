---
title: "PivotFieldCollection.AddByBaseIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotFieldCollection. Agrega un objeto PivotField al tipo específico PivotFields"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldcollection/addbybaseindex/
---
## PivotFieldCollection.AddByBaseIndex method

Agrega un objeto PivotField al tipo específico PivotFields.

```csharp
public int AddByBaseIndex(int baseFieldIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baseFieldIndex | Int32 | índice del campo en los PivotFields base. |

### Valor de retorno

el índice del objeto PivotField en estos PivotFields.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodAddByBaseIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de ejemplo
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Year";
            worksheet.Cells["B2"].Value = 2022;
            worksheet.Cells["B3"].Value = 2023;
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C3", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Agregar campos iniciales
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Agregar el campo Año al área de filas usando AddByBaseIndex
            int newIndex = pivotTable.RowFields.AddByBaseIndex(1);
            Console.WriteLine("Added field at index: " + newIndex);

            workbook.Save("PivotFieldAddByBaseIndexDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


