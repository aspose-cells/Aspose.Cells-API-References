---
title: "WorkbookSettings.ShowTabs"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "WorkbookSettings property. Obtiene o establece un valor que indica si se muestran las pestañas del Libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbooksettings/showtabs/
---
## WorkbookSettings.ShowTabs property

Obtiene o establece un valor que indica si se muestran las pestañas del Workbook.

```csharp
public bool ShowTabs { get; set; }
```

### Observaciones

El valor predeterminado es true.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyShowTabsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Ocultar las pestañas de la hoja de cálculo
            workbook.Settings.ShowTabs = false;
            
            // Guarda el libro de trabajo
            workbook.Save("HideTabsDemo.xlsx", SaveFormat.Xlsx);
            
            // Crear otro libro de trabajo para mostrar las pestañas
            Workbook workbook2 = new Workbook();
            
            // Asegurar que las pestañas sean visibles (el valor predeterminado es true)
            workbook2.Settings.ShowTabs = true;
            
            // Guarda el libro de trabajo
            workbook2.Save("ShowTabsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


