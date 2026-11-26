---
title: "WorkbookSettings.PaperSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene y establece el tamaño de papel de impresión predeterminado"
type: docs
url: /es/net/aspose.cells/workbooksettings/papersize/
---
## WorkbookSettings.PaperSize property

Obtiene y establece el tamaño de papel de impresión predeterminado.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Observaciones

Si no hay una configuración sobre el tamaño de papel, MS Excel usará la configuración predeterminada de la impresora.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer el tamaño de papel a A5
            workbook.Settings.PaperSize = PaperSizeType.PaperA5;
            
            // Verificar que el tamaño de papel esté configurado correctamente en la primera hoja de cálculo
            Console.WriteLine("Paper size: " + workbook.Worksheets[0].PageSetup.PaperSize);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [PaperSizeType](../../papersizetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


