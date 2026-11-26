---
title: "ListObject.ShowTotals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Obtiene y establece si esta tabla muestra la fila de totales"
type: docs
url: /es/net/aspose.cells.tables/listobject/showtotals/
---
## ListObject.ShowTotals property

Obtiene y establece si esta TAble muestra la fila total.

```csharp
public bool ShowTotals { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTotalsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para crear una tabla
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(8);

            // Crear un objeto de lista o tabla
            int index = worksheet.ListObjects.Add("A1", "B4", true);
            ListObject table = worksheet.ListObjects[index];

            // Habilitar fila de totales y establecer un cálculo
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Guarda el libro de trabajo
            workbook.Save("ListObjectShowTotalsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


