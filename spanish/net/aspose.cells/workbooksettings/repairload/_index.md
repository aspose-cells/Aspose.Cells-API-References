---
title: "WorkbookSettings.RepairLoad"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "WorkbookSettings property. Indica si la aplicación abrió el libro de trabajo por última vez en modo seguro o de reparación"
type: docs
url: /es/net/aspose.cells/workbooksettings/repairload/
---
## WorkbookSettings.RepairLoad property

Indica si la aplicación abrió por última vez el workbook en modo seguro o de reparación.

```csharp
public bool RepairLoad { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRepairLoadDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Configurar la configuración del libro
            workbook.Settings.AutoRecover = false;
            workbook.Settings.DataExtractLoad = true;
            workbook.Settings.CrashSave = true;
            workbook.Settings.RepairLoad = true;

            // Guarda el libro de trabajo
            string outputPath = "WorkbookSettings_RepairLoad_Example.xlsx";
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


