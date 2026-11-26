---
title: "WorkbookSettings.Shared"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene o establece un valor que indica si el libro de trabajo está compartido"
type: docs
url: /es/net/aspose.cells/workbooksettings/shared/
---
## WorkbookSettings.Shared property

Obtiene o establece un valor que indica si el Workbook está compartido.

```csharp
public bool Shared { get; set; }
```

### Observaciones

El valor predeterminado es false.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySharedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook book = new Workbook();
            
            // Establecer la propiedad Shared a true
            book.Settings.Shared = true;
            
            // Guarda el libro de trabajo
            string outputPath = "output_shared.xlsx";
            book.Save(outputPath);
            
            // Cargar el libro de trabajo guardado para verificar la propiedad Shared
            Workbook loadedBook = new Workbook(outputPath);
            Console.WriteLine("Shared property value: " + loadedBook.Settings.Shared);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


