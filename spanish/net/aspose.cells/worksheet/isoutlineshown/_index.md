---
title: "Worksheet.IsOutlineShown"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Indica si se debe mostrar el contorno"
type: docs
url: /es/net/aspose.cells/worksheet/isoutlineshown/
---
## Worksheet.IsOutlineShown property

Indica si se muestra el contorno.

```csharp
public bool IsOutlineShown { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsOutlineShownDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establezca que se muestre el contorno
            worksheet.IsOutlineShown = true;
            Console.WriteLine("Outline shown: " + worksheet.IsOutlineShown);
            
            // Guarde y vuelva a cargar para demostrar la persistencia
            string filePath = "IsOutlineShownDemo.xlsx";
            workbook.Save(filePath);
            
            Workbook loadedWorkbook = new Workbook(filePath);
            Console.WriteLine("Reloaded - Outline shown: " + loadedWorkbook.Worksheets[0].IsOutlineShown);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


