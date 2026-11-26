---
title: "Worksheet.CodeName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene el nombre de código de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/codename/
---
## Worksheet.CodeName property

Obtiene el nombre de código de la hoja de cálculo.

```csharp
public string CodeName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCodeNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Muestra el CodeName predeterminado
            Console.WriteLine("Default CodeName: " + worksheet.CodeName);
            
            // Cambia el CodeName
            worksheet.CodeName = "MySheet";
            Console.WriteLine("Modified CodeName: " + worksheet.CodeName);
            
            // Agrega una nueva hoja de cálculo y muestra su CodeName
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            Console.WriteLine("New Sheet CodeName: " + newSheet.CodeName);
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetCodeNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


