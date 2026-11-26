---
title: "WorkbookDesigner.UpdateEmptyStringAsNull"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookDesigner. Si TRUE, se insertará Null si el valor es"
type: docs
url: /es/net/aspose.cells/workbookdesigner/updateemptystringasnull/
---
## WorkbookDesigner.UpdateEmptyStringAsNull property

Si TRUE, se insertará Null si el valor es "";

```csharp
public bool UpdateEmptyStringAsNull { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyUpdateEmptyStringAsNullDemo
    {
        public static void Run()
        {
            // Crear un DataSet de ejemplo con cadenas vacías
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("Name");
            dt.Columns.Add("Price");
            dt.Rows.Add("Laptop", "");
            dt.Rows.Add("", "999.99");
            ds.Tables.Add(dt);

            // Crear un libro de trabajo con marcadores de diseñador
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&=$Products.Name");
            worksheet.Cells["B1"].PutValue("&=$Products.Price");

            // Inicializar WorkbookDesigner y establecer propiedades
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.UpdateEmptyStringAsNull = true; // This is the key property being demonstrated
            
            // Establecer origen de datos y procesar
            designer.SetDataSource(ds.Tables["Products"]);
            designer.Process();

            // Verificar resultados
            Console.WriteLine("A1 value: " + worksheet.Cells["A1"].StringValue); // Should show "Laptop"
            Console.WriteLine("B1 value: " + worksheet.Cells["B1"].StringValue); // Should show empty (null)
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


