---
title: "WorkbookSettings.UpdateLinksType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene y establece cómo se actualizan los enlaces externos cuando se abre el libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbooksettings/updatelinkstype/
---
## WorkbookSettings.UpdateLinksType property

Obtiene y establece cómo se actualizan los enlaces externos cuando se abre el libro de trabajo.

```csharp
public UpdateLinksType UpdateLinksType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateLinksTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establezca UpdateLinksType a Never
            workbook.Settings.UpdateLinksType = UpdateLinksType.Never;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Cargar el libro guardado para verificar la configuración
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Muestre el valor de UpdateLinksType
            Console.WriteLine("UpdateLinksType: " + loadedWorkbook.Settings.UpdateLinksType);
        }
    }
}
```

### Ver también

* enum [UpdateLinksType](../../updatelinkstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


