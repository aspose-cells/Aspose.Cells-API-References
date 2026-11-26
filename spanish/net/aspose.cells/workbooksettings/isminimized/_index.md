---
title: "WorkbookSettings.IsMinimized"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Representa si la hoja de cálculo generada se abrirá minimizada"
type: docs
url: /es/net/aspose.cells/workbooksettings/isminimized/
---
## WorkbookSettings.IsMinimized property

Representa si la hoja de cálculo generada se abrirá minimizada.

```csharp
public bool IsMinimized { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsMinimizedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Establecer la propiedad IsMinimized a true
            workbook.Settings.IsMinimized = true;

            // Guarda el libro de trabajo
            workbook.Save("IsMinimizedDemo.xlsx");

            // Cargar el libro de trabajo guardado para verificar la propiedad
            Workbook loadedWorkbook = new Workbook("IsMinimizedDemo.xlsx");

            // Mostrar el valor de la propiedad IsMinimized
            Console.WriteLine("Workbook IsMinimized property: " + loadedWorkbook.Settings.IsMinimized);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


