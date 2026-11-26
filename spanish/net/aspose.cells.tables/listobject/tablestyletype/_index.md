---
title: "ListObject.TableStyleType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Obtiene el estilo de tabla incorporado"
type: docs
url: /es/net/aspose.cells.tables/listobject/tablestyletype/
---
## ListObject.TableStyleType property

Obtiene y el estilo de tabla incorporado.

```csharp
public TableStyleType TableStyleType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyTableStyleTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i+1}-{j+1}");
                }
            }
            
            // Obtener la colección de objetos de lista
            ListObjectCollection tables = worksheet.ListObjects;
            
            // Agregar una tabla
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[0];
            
            // Establecer el estilo de tabla
            table.TableStyleType = TableStyleType.TableStyleDark2;
            
            // Guarda el libro de trabajo
            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TableStyleType](../../tablestyletype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


