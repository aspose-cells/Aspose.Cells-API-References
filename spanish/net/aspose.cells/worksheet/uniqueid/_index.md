---
title: "Worksheet.UniqueId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene y establece el id único, es el mismo que 15DB5C3CA5A148AF8F253D86AC232D4F"
type: docs
url: /es/net/aspose.cells/worksheet/uniqueid/
---
## Worksheet.UniqueId property

Obtiene y establece el id único, es el mismo que {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.

```csharp
public string UniqueId { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyUniqueIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Generar un ID único para la hoja de cálculo
            string uniqueId = "{" + Guid.NewGuid().ToString() + "}";
            
            // Establecer la propiedad UniqueId de la primera hoja de cálculo
            workbook.Worksheets[0].UniqueId = uniqueId;
            
            // Guarda el libro de trabajo
            string outputPath = "SheetUniqueIdDemo.xlsx";
            workbook.Save(outputPath);
            
            // Recargar el libro de trabajo para verificar que el UniqueId persista
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Mostrar el UniqueId para demostrar la funcionalidad
            Console.WriteLine("Worksheet UniqueId: " + loadedWorkbook.Worksheets[0].UniqueId);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


