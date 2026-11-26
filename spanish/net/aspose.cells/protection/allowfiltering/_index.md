---
title: "Protection.AllowFiltering"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Protection. Representa si el usuario puede usar un AutoFilter que se creó antes de que la hoja estuviera protegida"
type: docs
url: /es/net/aspose.cells/protection/allowfiltering/
---
## Protection.AllowFiltering property

Representa si se permite al usuario usar un AutoFiltro que se creó antes de que la hoja fuera protegida.

```csharp
public bool AllowFiltering { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFilteringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Habilitar la protección de la hoja de cálculo
            worksheet.Protect(ProtectionType.All);
            
            // Establecer la propiedad AllowFiltering a verdadero
            worksheet.Protection.AllowFiltering = true;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Verificar que la propiedad se guardó correctamente
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AllowFiltering: " + 
                loadedWorkbook.Worksheets[0].Protection.AllowFiltering);
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


