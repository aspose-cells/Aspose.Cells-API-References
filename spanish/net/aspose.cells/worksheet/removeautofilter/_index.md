---
title: "Worksheet.RemoveAutoFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Elimina el filtro automático de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/removeautofilter/
---
## Worksheet.RemoveAutoFilter method

Elimina el filtro automático de la hoja de cálculo.

```csharp
public void RemoveAutoFilter()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveAutoFilterDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            
            // Aplicar filtro automático
            worksheet.AutoFilter.Range = "A1:A3";
            
            Console.WriteLine("AutoFilter applied: " + worksheet.HasAutofilter);
            
            // Eliminar filtro automático
            worksheet.RemoveAutoFilter();
            
            Console.WriteLine("AutoFilter after removal: " + worksheet.HasAutofilter);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


