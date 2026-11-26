---
title: "WorkbookSettings.Author"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "WorkbookSettings property. Obtiene y establece el autor del archivo"
type: docs
url: /es/net/aspose.cells/workbooksettings/author/
---
## WorkbookSettings.Author property

Obtiene y establece el autor del archivo.

```csharp
public string Author { get; set; }
```

### Observaciones

No está configurado, verifica primero [`Author`](../../../aspose.cells.properties/builtindocumentpropertycollection/author/), luego verifica el usuario del Entorno.

### Ejemplos

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAuthorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Establecer la propiedad author
            settings.Author = "John Doe";

            // Agregar algunos datos de muestra para demostrar la funcionalidad del libro de trabajo
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Sample Workbook");
            sheet.Cells["A2"].PutValue("Created by: " + settings.Author);
            sheet.Cells["A3"].PutValue(DateTime.Now.ToString());

            // Guarda el libro de trabajo
            workbook.Save("AuthorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


