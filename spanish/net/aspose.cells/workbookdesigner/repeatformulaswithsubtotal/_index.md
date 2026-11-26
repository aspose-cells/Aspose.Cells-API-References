---
title: "WorkbookDesigner.RepeatFormulasWithSubtotal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookDesigner. Indica si se repiten fórmulas con fila de subtotal"
type: docs
url: /es/net/aspose.cells/workbookdesigner/repeatformulaswithsubtotal/
---
## WorkbookDesigner.RepeatFormulasWithSubtotal property

Indica si se repiten fórmulas con fila de subtotal.

```csharp
public bool RepeatFormulasWithSubtotal { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyRepeatFormulasWithSubtotalDemo
    {
        public static void Run()
        {
            // Crear un DataTable de ejemplo
            DataTable dt = new DataTable("products1");
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("ProductName", typeof(string));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            dt.Columns.Add("Quantity", typeof(int));
            
            // Agregar datos de ejemplo
            dt.Rows.Add(1, "Product A", 10.5m, 5);
            dt.Rows.Add(2, "Product B", 15.2m, 3);
            dt.Rows.Add(3, "Product C", 8.7m, 7);

            // Crear un nuevo libro de trabajo con una fórmula de plantilla
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Configurar la plantilla con marcadores inteligentes y fórmula
            worksheet.Cells["A1"].PutValue("&=$ProductID");
            worksheet.Cells["B1"].PutValue("&=$ProductName");
            worksheet.Cells["C1"].PutValue("&=$UnitPrice");
            worksheet.Cells["D1"].PutValue("&=$Quantity");
            worksheet.Cells["E1"].PutValue("=SUM(C2:D2)"); // Formula to be repeated

            // Crear diseñador y establecer RepeatFormulasWithSubtotal
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            designer.RepeatFormulasWithSubtotal = true;
            designer.SetDataSource(dt);
            
            // Procesar la plantilla
            designer.Process();

            // Verificar que la fórmula se repitió en cada fila
            Console.WriteLine("Formula in E2: " + worksheet.Cells["E2"].Formula);
            Console.WriteLine("Formula in E3: " + worksheet.Cells["E3"].Formula);
            Console.WriteLine("Formula in E4: " + worksheet.Cells["E4"].Formula);

            // Guardar el resultado
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


