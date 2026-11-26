---
title: "Worksheet.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Worksheet propiedad. Obtiene o establece el nombre de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/name/
---
## Worksheet.Name property

Obtiene o establece el nombre de la hoja de cálculo.

```csharp
public string Name { get; set; }
```

### Observaciones

La longitud máxima del nombre de la hoja es 31. Y no puedes asignar el mismo nombre (sin distinción de mayúsculas) a dos hojas de cálculo. Por ejemplo, no puedes establecer "SheetName1" en la primera hoja y establecer "SHEETNAME1" en la segunda hoja.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Accede a la primera hoja y establece su nombre
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Añade una nueva hoja con un nombre específico
            Worksheet newSheet = workbook.Worksheets.Add("ReportSheet");
            
            // Muestra los nombres de todas las hojas
            Console.WriteLine("Worksheet Names:");
            foreach (Worksheet ws in workbook.Worksheets)
            {
                Console.WriteLine(ws.Name);
            }
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetNamesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


