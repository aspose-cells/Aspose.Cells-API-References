---
title: "WorkbookSettings.MemorySetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene o establece las opciones de uso de memoria. La nueva opción se tomará como la opción predeterminada para las hojas de cálculo recién creadas, pero no tendrá efecto en las hojas de cálculo existentes."
type: docs
url: /es/net/aspose.cells/workbooksettings/memorysetting/
---
## WorkbookSettings.MemorySetting property

Obtiene o establece las opciones de uso de memoria. La nueva opción se tomará como la opción predeterminada para las hojas de cálculo recién creadas, pero no tendrá efecto en las hojas de cálculo existentes.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Observaciones

Para obtener más detalles sobre el modo de memoria, consulte [`MemorySetting`](../../cells/memorysetting/).

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo con la configuración de preferencia de memoria
            Workbook wb = new Workbook();
            wb.Settings.MemorySetting = MemorySetting.MemoryPreference;
            
            // Acceder a la primera hoja de cálculo y agregar algunos datos
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Memory Setting Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Guarde en un flujo de memoria con formato PDF
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Pdf);
                Console.WriteLine("Workbook saved to PDF with MemoryPreference setting");
            }
        }
    }
}
```

### Ver también

* enum [MemorySetting](../../memorysetting/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


