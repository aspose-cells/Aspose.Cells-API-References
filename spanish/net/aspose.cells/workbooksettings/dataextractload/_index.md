---
title: "WorkbookSettings.DataExtractLoad"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Indica si la aplicación abrió por última vez el libro para recuperación de datos"
type: docs
url: /es/net/aspose.cells/workbooksettings/dataextractload/
---
## WorkbookSettings.DataExtractLoad property

Indica si la aplicación abrió por última vez el libro para recuperación de datos.

```csharp
public bool DataExtractLoad { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDataExtractLoadDemo
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
            string destPath = "output.xlsx";
            workbook.Save(destPath);
            
            // Recargar el libro para verificar la configuración
            Workbook loadedWorkbook = new Workbook(destPath);
            
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


