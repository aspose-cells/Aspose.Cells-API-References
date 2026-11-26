---
title: "ImageOrPrintOptions.PrintWithStatusDialog"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Si PrintWithStatusDialog es true, habrá un diálogo que muestra el estado actual de la impresión. de lo contrario, no se mostrará ningún diálogo."
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/
---
## ImageOrPrintOptions.PrintWithStatusDialog property

Si PrintWithStatusDialog = true, aparecerá un diálogo que muestra el estado actual de la impresión. De lo contrario, no se mostrará ningún diálogo.

```csharp
public bool PrintWithStatusDialog { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using System.Threading;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPrintWithStatusDialogDemo
    {
        public static void Run()
        {
            // Inicializar un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Establecer opciones de imagen o impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintWithStatusDialog = false; // Disable print status dialog
            options.PageIndex = 0;
            options.PageCount = 1;

            // Crear renderizado de hoja
            SheetRender sheetRender = new SheetRender(worksheet, options);
            
            // Imprimir a PDF
            sheetRender.ToImage(0, "output.png");

            // Esperar a la creación del archivo (lógica de espera simplificada)
            int attempts = 0;
            while (!File.Exists("output.png") && attempts < 5)
            {
                Thread.Sleep(1000);
                attempts++;
            }

            if (File.Exists("output.png"))
            {
                Console.WriteLine("Image file created successfully");
            }
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


