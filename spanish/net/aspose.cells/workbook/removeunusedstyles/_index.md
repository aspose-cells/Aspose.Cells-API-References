---
title: "Workbook.RemoveUnusedStyles"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Elimina todos los estilos no utilizados"
type: docs
url: /es/net/aspose.cells/workbook/removeunusedstyles/
---
## Workbook.RemoveUnusedStyles method

Elimina todos los estilos no utilizados.

```csharp
public void RemoveUnusedStyles()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveUnusedStylesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = wb.Worksheets[0];
            
            // Agregue algunos datos de muestra con estilos
            for (int i = 0; i < 10; i++)
            {
                Cell cell = sheet.Cells[i, 0];
                cell.PutValue("Item " + (i + 1));
                
                // Aplique diferentes estilos a las celdas
                Style style = wb.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 10 + i;
                style.Font.IsBold = i % 2 == 0;
                cell.SetStyle(style);
            }
            
            // Elimine algunas celdas para dejar estilos no utilizados
            sheet.Cells.DeleteRows(5, 5);
            
            // Guarde antes de eliminar los estilos no utilizados
            wb.Save("BeforeRemoveUnusedStyles.xlsx");
            
            // Eliminar estilos no utilizados
            wb.RemoveUnusedStyles();
            
            // Guardar después de eliminar estilos no utilizados
            wb.Save("AfterRemoveUnusedStyles.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


