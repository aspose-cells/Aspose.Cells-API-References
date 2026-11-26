---
title: "WorkbookSettings.IsVScrollBarVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene o establece un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento vertical"
type: docs
url: /es/net/aspose.cells/workbooksettings/isvscrollbarvisible/
---
## WorkbookSettings.IsVScrollBarVisible property

Obtiene o establece un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento vertical.

```csharp
public bool IsVScrollBarVisible { get; set; }
```

### Observaciones

El valor predeterminado es true.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsVScrollBarVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;
            
            // Ocultar la barra de desplazamiento vertical
            settings.IsVScrollBarVisible = false;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Vertical scroll bar visibility set to false. Workbook saved.");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


