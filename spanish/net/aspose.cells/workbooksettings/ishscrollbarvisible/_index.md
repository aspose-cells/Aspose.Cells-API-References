---
title: "WorkbookSettings.IsHScrollBarVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene o establece un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento horizontal"
type: docs
url: /es/net/aspose.cells/workbooksettings/ishscrollbarvisible/
---
## WorkbookSettings.IsHScrollBarVisible property

Obtiene o establece un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento horizontal.

```csharp
public bool IsHScrollBarVisible { get; set; }
```

### Observaciones

El valor predeterminado es true.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHScrollBarVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;
            
            // Ocultar la barra de desplazamiento horizontal
            settings.IsHScrollBarVisible = false;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with horizontal scroll bar hidden.");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


