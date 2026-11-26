---
title: "PageSetup.PrinterSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Obtiene y establece la configuración de la impresora predeterminada"
type: docs
url: /es/net/aspose.cells/pagesetup/printersettings/
---
## PageSetup.PrinterSettings property

Obtiene y establece la configuración de la impresora predeterminada.

```csharp
public byte[] PrinterSettings { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrinterSettingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Test Printer Settings");
            
            // Acceder a la configuración de página
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Establecer la configuración de la impresora (como matriz de bytes)
            byte[] printerSettings = new byte[10]; // Simplified example
            pageSetup.PrinterSettings = printerSettings;
            
            // Verificar que la configuración de la impresora esté establecida
            Console.WriteLine("Printer Settings: " + (pageSetup.PrinterSettings != null));
            
            // Guarda el libro de trabajo
            workbook.Save("PrinterSettingsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


