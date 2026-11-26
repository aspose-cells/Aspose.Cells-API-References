---
title: "WorkbookSettings.CheckCustomNumberFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Indica si se verifica el formato numérico personalizado al establecer Style.Custom"
type: docs
url: /es/net/aspose.cells/workbooksettings/checkcustomnumberformat/
---
## WorkbookSettings.CheckCustomNumberFormat property

Indica si se verifica el formato numérico personalizado al establecer Style.Custom.

```csharp
public bool CheckCustomNumberFormat { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckCustomNumberFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            
            // Primero establezca un formato numérico personalizado válido
            style.Custom = "#,##0.00";
            
            // Habilitar la verificación estricta
            workbook.Settings.CheckCustomNumberFormat = true;
            
            try
            {
                // Intentar establecer un formato numérico personalizado inválido
                style.Custom = "fff @ ggg";
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error setting custom format: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


