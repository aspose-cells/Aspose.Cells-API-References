---
title: "Worksheet.ClearComments"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Elimina todos los comentarios en la hoja de cálculo del diseñador"
type: docs
url: /es/net/aspose.cells/worksheet/clearcomments/
---
## Worksheet.ClearComments method

Elimina todos los comentarios en la hoja de cálculo del diseñador.

```csharp
public void ClearComments()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodClearCommentsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar comentarios de muestra a las celdas usando referencias de celda
            int comment1 = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1].Note = "This is comment 1";
            
            int comment2 = worksheet.Comments.Add("B3");
            worksheet.Comments[comment2].Note = "This is comment 2";
            
            int comment3 = worksheet.Comments.Add("C5");
            worksheet.Comments[comment3].Note = "This is comment 3";

            // Mostrar el recuento de comentarios antes de eliminar
            Console.WriteLine($"Comments count before ClearComments(): {worksheet.Comments.Count}");

            // Eliminar todos los comentarios de la hoja de cálculo
            worksheet.ClearComments();

            // Mostrar el recuento de comentarios después de eliminar
            Console.WriteLine($"Comments count after ClearComments(): {worksheet.Comments.Count}");

            // Guarda el libro de trabajo
            workbook.Save("ClearCommentsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


