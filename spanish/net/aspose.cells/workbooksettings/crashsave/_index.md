---
title: "WorkbookSettings.CrashSave"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "propiedad WorkbookSettings. indica si la aplicación guardó por última vez el archivo del libro después de un fallo"
type: docs
url: /es/net/aspose.cells/workbooksettings/crashsave/
---
## WorkbookSettings.CrashSave property

Indica si la aplicación guardó por última vez el archivo del libro después de un bloqueo.

```csharp
public bool CrashSave { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCrashSaveDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("CrashSave Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;

            // Demostrar la propiedad CrashSave
            settings.CrashSave = true;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // Guardar con guardado de fallos habilitado
            workbook.Save("CrashSaveEnabled.xlsx");

            // Desactivar el guardado de fallos
            settings.CrashSave = false;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // Guardar con guardado de fallos deshabilitado
            workbook.Save("CrashSaveDisabled.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


