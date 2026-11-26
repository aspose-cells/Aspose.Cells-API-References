---
title: "ListColumn.TotalsCalculation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListColumn. Obtiene y establece el tipo de cálculo en la fila Totals de la columna de lista"
type: docs
url: /es/net/aspose.cells.tables/listcolumn/totalscalculation/
---
## ListColumn.TotalsCalculation property

Obtiene y establece el tipo de cálculo en la fila Totals de la columna de lista.

```csharp
public TotalsCalculation TotalsCalculation { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyTotalsCalculationDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("Item 3");
            worksheet.Cells["B4"].PutValue(200);

            // Crear un objeto de lista
            int listObjIndex = worksheet.ListObjects.Add(0, 0, 4, 1, true);
            ListObject listObj = worksheet.ListObjects[listObjIndex];
            listObj.ShowTotals = true;
            
            // Establezca el cálculo de totales para la segunda columna
            listObj.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Guarda el libro de trabajo
            workbook.Save("ListColumnTotalsCalculationDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TotalsCalculation](../../totalscalculation/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


