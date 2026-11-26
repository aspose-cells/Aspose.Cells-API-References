---
title: "WorkbookDesigner.UpdateReference"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookDesigner. Indica si las referencias en otras hojas de cálculo serán actualizadas"
type: docs
url: /es/net/aspose.cells/workbookdesigner/updatereference/
---
## WorkbookDesigner.UpdateReference property

Indica si las referencias en otras hojas de cálculo se actualizarán.

```csharp
public bool UpdateReference { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Crear un conjunto de datos de ejemplo
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("ID", typeof(int));
            dt.Columns.Add("Name", typeof(string));
            dt.Columns.Add("Price", typeof(decimal));
            
            dt.Rows.Add(1, "Product A", 19.99);
            dt.Rows.Add(2, "Product B", 29.99);
            dt.Rows.Add(3, "Product C", 39.99);
            
            ds.Tables.Add(dt);

            // Crear un diseñador de libros de trabajo
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Establecer la propiedad UpdateReference a true
            designer.UpdateReference = true;
            
            // Crear un nuevo libro de trabajo con una plantilla
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar marcadores inteligentes
            worksheet.Cells["A1"].PutValue("&=Products.ID");
            worksheet.Cells["B1"].PutValue("&=Products.Name");
            worksheet.Cells["C1"].PutValue("&=Products.Price");
            
            designer.Workbook = workbook;
            designer.SetDataSource("Products", dt);
            
            // Procesar el diseñador
            designer.Process();
            
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


