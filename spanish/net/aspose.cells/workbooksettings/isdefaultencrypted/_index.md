---
title: "WorkbookSettings.IsDefaultEncrypted"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Indica si se cifra el libro con la contraseña predeterminada cuando la estructura y las ventanas del libro están bloqueadas"
type: docs
url: /es/net/aspose.cells/workbooksettings/isdefaultencrypted/
---
## WorkbookSettings.IsDefaultEncrypted property

Indica si se cifra el libro con la contraseña predeterminada cuando la estructura y las ventanas del libro están bloqueadas.

```csharp
public bool IsDefaultEncrypted { get; set; }
```

### Observaciones

El valor predeterminado es false ahora. Es lo mismo que MS Excel 2013.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsDefaultEncryptedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Console.WriteLine("IsDefaultEncrypted: " + workbook.Settings.IsDefaultEncrypted);
            
            workbook.Settings.IsDefaultEncrypted = true;
            Console.WriteLine("After setting to true: " + workbook.Settings.IsDefaultEncrypted);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


