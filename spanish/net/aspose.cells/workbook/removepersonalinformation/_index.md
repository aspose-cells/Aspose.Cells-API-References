---
title: "Workbook.RemovePersonalInformation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Elimina información personal"
type: docs
url: /es/net/aspose.cells/workbook/removepersonalinformation/
---
## Workbook.RemovePersonalInformation method

Elimina información personal.

```csharp
public void RemovePersonalInformation()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemovePersonalInformationDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Agregar un comentario con información del autor
            int commentIndex = sheet.Comments.Add("A1");
            sheet.Comments[commentIndex].Note = "Sample comment";
            sheet.Comments[commentIndex].Author = "Test Author";
            
            // Mostrar información del autor original
            Console.WriteLine("Before removal - Comment Author: " + sheet.Comments[commentIndex].Author);
            
            // Eliminar información personal
            wb.RemovePersonalInformation();
            
            // Guarda el libro de trabajo
            wb.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Recargar para verificar la eliminación
            Workbook wb2 = new Workbook("output.xlsx");
            Console.WriteLine("After removal - Comment Author: " + wb2.Worksheets[0].Comments[commentIndex].Author);
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


