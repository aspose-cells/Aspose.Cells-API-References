---
title: "SaveOptions.WarningCallback"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SaveOptions. Obtiene o establece la devolución de llamada de advertencia"
type: docs
url: /es/net/aspose.cells/saveoptions/warningcallback/
---
## SaveOptions.WarningCallback property

Obtiene o establece la devolución de llamada de advertencia.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data");

            // Crear opciones de guardado
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Establecer devolución de llamada de advertencia personalizada
            saveOptions.WarningCallback = new CustomWarningCallback();

            // Esto generará una advertencia sobre una característica no compatible en formato HTML
            worksheet.PageSetup.PrintTitleRows = "$1:$1";

            // Guardar con opciones que podrían generar advertencias
            workbook.Save("WarningCallbackDemo.html", saveOptions);
        }
    }

    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // Manejar la advertencia - en este caso simplemente mostrarla
            Console.WriteLine($"Warning: {warningInfo.Description}");
            Console.WriteLine($"Warning type: {warningInfo.WarningType}");
        }
    }
}
```

### Ver también

* interface [IWarningCallback](../../iwarningcallback/)
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


