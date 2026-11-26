---
title: "Worksheet.TabId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Especifica el identificador interno de la hoja"
type: docs
url: /es/net/aspose.cells/worksheet/tabid/
---
## Worksheet.TabId property

Especifica el identificador interno de la hoja.

```csharp
public int TabId { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer la propiedad TabId
            worksheet.TabId = 107;
            
            // Guarda el libro de trabajo
            string outputPath = "output.xlsb";
            workbook.Save(outputPath);
            
            // Cargar el libro guardado para verificar el TabId
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Mostrar el valor de TabId
            Console.WriteLine("Worksheet TabId: " + loadedWorksheet.TabId);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


