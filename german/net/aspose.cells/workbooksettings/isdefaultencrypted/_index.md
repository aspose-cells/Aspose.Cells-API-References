---
title: "WorkbookSettings.IsDefaultEncrypted"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt an, ob die Arbeitsmappe mit dem Standardkennwort verschlüsselt wird, wenn Struktur und Fenster der Arbeitsmappe gesperrt sind."
type: docs
url: /de/net/aspose.cells/workbooksettings/isdefaultencrypted/
---
## WorkbookSettings.IsDefaultEncrypted property

Gibt an, ob das Workbook mit dem Standardpasswort verschlüsselt wird, wenn Struktur und Fenster des Workbooks gesperrt sind.

```csharp
public bool IsDefaultEncrypted { get; set; }
```

### Hinweise

Der Standardwert ist jetzt false. Er ist derselbe wie bei MS Excel 2013.

### Beispiele

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

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


