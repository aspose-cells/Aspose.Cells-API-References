---
title: "ListColumn.SetDataStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ListColumn. Establece el estilo de los datos en esta columna de la tabla"
type: docs
url: /es/net/aspose.cells.tables/listcolumn/setdatastyle/
---
## ListColumn.SetDataStyle method

Establece el estilo de los datos en esta columna de la tabla.

```csharp
public void SetDataStyle(Style style)
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListColumnMethodSetDataStyleWithStyleDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            
            // Crear un objeto lista (tabla)
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            
            // Obtenga el estilo de la primera columna
            Style style = table.ListColumns[0].GetDataStyle();
            
            // Modificar el estilo
            style.Pattern = BackgroundType.Solid;
            style.BackgroundColor = System.Drawing.Color.Red;
            
            // Aplique el estilo modificado a la columna
            table.ListColumns[0].SetDataStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../../aspose.cells/style/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


