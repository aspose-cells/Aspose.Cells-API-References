---
title: "WorkbookSettings.AutoRecover"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Indica si el archivo está marcado para autorrecuperación"
type: docs
url: /es/net/aspose.cells/workbooksettings/autorecover/
---
## WorkbookSettings.AutoRecover property

Indica si el archivo está marcado para recuperación automática.

```csharp
public bool AutoRecover { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAutoRecoverDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer AutoRecover y otras configuraciones
            workbook.Settings.AutoRecover = false;
            workbook.Settings.DataExtractLoad = true;
            workbook.Settings.CrashSave = true;
            workbook.Settings.RepairLoad = true;

            // Guarda el libro de trabajo
            string outputPath = "WorkbookSettings_AutoRecoverDemo.xlsx";
            workbook.Save(outputPath);

            // Cargar el libro de trabajo guardado para verificar la configuración
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Mostrar la configuración en la consola
            Console.WriteLine("AutoRecover: " + loadedWorkbook.Settings.AutoRecover);
            Console.WriteLine("DataExtractLoad: " + loadedWorkbook.Settings.DataExtractLoad);
            Console.WriteLine("CrashSave: " + loadedWorkbook.Settings.CrashSave);
            Console.WriteLine("RepairLoad: " + loadedWorkbook.Settings.RepairLoad);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


