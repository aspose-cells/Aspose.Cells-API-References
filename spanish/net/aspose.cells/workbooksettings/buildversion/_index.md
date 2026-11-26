---
title: "WorkbookSettings.BuildVersion"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Especifica la versión pública incremental de la aplicación"
type: docs
url: /es/net/aspose.cells/workbooksettings/buildversion/
---
## WorkbookSettings.BuildVersion property

Especifica la versión incremental pública de la aplicación.

```csharp
public string BuildVersion { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyBuildVersionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Establecer configuraciones básicas
            settings.Author = "Sample Author";
            settings.CultureInfo = new CultureInfo("en-US");
            
            // Demostrar la propiedad BuildVersion
            settings.BuildVersion = "2.5.0";
            Console.WriteLine($"Build Version set to: {settings.BuildVersion}");
            
            // Guarda el libro de trabajo
            workbook.Save("BuildVersionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


