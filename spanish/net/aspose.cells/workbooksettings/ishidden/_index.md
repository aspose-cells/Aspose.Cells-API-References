---
title: "WorkbookSettings.IsHidden"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Indica si este libro de trabajo está oculto"
type: docs
url: /es/net/aspose.cells/workbooksettings/ishidden/
---
## WorkbookSettings.IsHidden property

Indica si este libro está oculto.

```csharp
public bool IsHidden { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;

            // Establezca la propiedad IsHidden en true
            settings.IsHidden = true;
            Console.WriteLine("Workbook is hidden: " + settings.IsHidden);

            // Guarda el libro de trabajo
            workbook.Save("WorkbookSettings_IsHidden_True.xlsx");

            // Cree otro libro de trabajo
            Workbook workbook2 = new Workbook();

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings2 = workbook2.Settings;

            // Establezca la propiedad IsHidden en false (predeterminado)
            settings2.IsHidden = false;
            Console.WriteLine("Workbook is hidden: " + settings2.IsHidden);

            // Guarda el libro de trabajo
            workbook2.Save("WorkbookSettings_IsHidden_False.xlsx");

            // Cargue y verifique los libros de trabajo guardados
            Workbook loadedWorkbook1 = new Workbook("WorkbookSettings_IsHidden_True.xlsx");
            Console.WriteLine("Loaded workbook1 is hidden: " + loadedWorkbook1.Settings.IsHidden);

            Workbook loadedWorkbook2 = new Workbook("WorkbookSettings_IsHidden_False.xlsx");
            Console.WriteLine("Loaded workbook2 is hidden: " + loadedWorkbook2.Settings.IsHidden);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


