---
title: "Name.Comment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Name. Obtiene y establece el comentario del nombre. Solo se aplica a Excel 2007 o versiones superiores."
type: docs
url: /es/net/aspose.cells/name/comment/
---
## Name.Comment property

Obtiene y establece el comentario del nombre. Solo se aplica a Excel 2007 o versiones superiores.

```csharp
public string Comment { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyCommentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un rango con nombre con comentario
            int index = workbook.Worksheets.Names.Add("TestRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
            namedRange.Comment = "This is a test named range";
            
            // Guarda el libro de trabajo
            workbook.Save("NamedRangeWithComment.xlsx");
            
            // Cargar el libro guardado para verificar el comentario
            Workbook loadedWorkbook = new Workbook("NamedRangeWithComment.xlsx");
            Name loadedNamedRange = loadedWorkbook.Worksheets.Names[0];
            
            // Mostrar el comentario para demostrar la funcionalidad
            Console.WriteLine("Named Range Comment: " + loadedNamedRange.Comment);
        }
    }
}
```

### Ver también

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


