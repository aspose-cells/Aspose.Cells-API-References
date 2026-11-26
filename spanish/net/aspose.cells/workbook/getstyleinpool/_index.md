---
title: "Workbook.GetStyleInPool"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Obtiene el estilo del grupo de estilos. Todos los estilos en el libro de trabajo se recopilarán en un grupo. Sólo hay un índice de referencia simple en las celdas"
type: docs
url: /es/net/aspose.cells/workbook/getstyleinpool/
---
## Workbook.GetStyleInPool method

Obtiene el estilo en el grupo de estilos. Todos los estilos del libro de trabajo se recopilarán en un grupo. Sólo hay un índice de referencia simple en las celdas.

```csharp
public Style GetStyleInPool(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice. |

### Valor de retorno

El estilo en el grupo corresponde al índice dado, puede ser nulo.

### Observaciones

Si el estilo devuelto se modifica, el estilo de todas las celdas (que hacen referencia a este estilo) se modificará.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetStyleInPoolWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Acceder a la primera hoja y agregar algunos datos de muestra
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123.45);
            ws.Cells["A3"].PutValue(DateTime.Now);
            
            // Aplicar algunos estilos
            Style style1 = wb.CreateStyle();
            style1.Custom = "$#,##0.00";
            ws.Cells["A2"].SetStyle(style1);
            
            Style style2 = wb.CreateStyle();
            style2.Custom = "yyyy-mm-dd";
            ws.Cells["A3"].SetStyle(style2);
            
            // Guardar en flujo de memoria
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                
                // Recargar libro de trabajo desde el flujo
                ms.Position = 0;
                Workbook reloadWb = new Workbook(ms);
                
                // Obtener y mostrar estilos del grupo de estilos
                int count = reloadWb.CountOfStylesInPool;
                Console.WriteLine($"Styles in pool: {count}");
                
                for (int i = 0; i < count; i++)
                {
                    Style style = reloadWb.GetStyleInPool(i);
                    Console.WriteLine($"Style {i}: CustomFormat={style.Custom}");
                }
            }
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


