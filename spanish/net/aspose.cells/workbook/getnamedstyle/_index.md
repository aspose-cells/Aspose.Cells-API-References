---
title: "Workbook.GetNamedStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Obtiene el estilo nombrado en el pool de estilos"
type: docs
url: /es/net/aspose.cells/workbook/getnamedstyle/
---
## Workbook.GetNamedStyle method

Obtiene el estilo nombrado en el grupo de estilos.

```csharp
public Style GetNamedStyle(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | nombre del estilo |

### Valor de retorno

estilo nombrado, puede ser nulo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetNamedStyleWithStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunos estilos nombrados
            Style style1 = workbook.CreateStyle();
            style1.Name = "Number7";
            style1.Custom = "#,##0.00";
            
            Style style2 = workbook.CreateStyle();
            style2.Name = "Center";
            style2.HorizontalAlignment = TextAlignmentType.Center;
            
            // Crear datos de ejemplo
            DataTable dt = new DataTable();
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("ProductName", typeof(string));
            dt.Columns.Add("Quantity", typeof(int));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            dt.Columns.Add("Discount", typeof(float));
            
            dt.Rows.Add(1, "Product A", 10, 19.99m, 0.1f);
            dt.Rows.Add(2, "Product B", 5, 29.99m, 0.15f);
            
            // Obtener hoja de cálculo y celdas
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Obtener estilos nombrados
            Style numberStyle = workbook.GetNamedStyle("Number7");
            Style centerStyle = workbook.GetNamedStyle("Center");
            
            // Aplicar estilos a los datos
            for(int i = 0; i < dt.Rows.Count; i++)
            {
                cells[i, 0].PutValue((int)dt.Rows[i]["ProductID"]);
                cells[i, 0].SetStyle(centerStyle);
                
                cells[i, 1].PutValue((string)dt.Rows[i]["ProductName"]);
                
                cells[i, 3].PutValue((decimal)dt.Rows[i]["UnitPrice"]);
                cells[i, 3].SetStyle(numberStyle);
            }
            
            // Guarda el libro de trabajo
            workbook.Save("GetNamedStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


