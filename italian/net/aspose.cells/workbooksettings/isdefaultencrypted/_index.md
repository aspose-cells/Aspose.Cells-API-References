---
title: "WorkbookSettings.IsDefaultEncrypted"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Indica se la cartella di lavoro è crittografata con la password predefinita quando la struttura e le finestre della cartella di lavoro sono bloccate"
type: docs
url: /it/net/aspose.cells/workbooksettings/isdefaultencrypted/
---
## WorkbookSettings.IsDefaultEncrypted property

Indica se crittografare la workbook con password predefinita se Structure e Windows della workbook sono bloccati.

```csharp
public bool IsDefaultEncrypted { get; set; }
```

### Osservazioni

Il valore predefinito è ora false. È lo stesso di MS Excel 2013.

### Esempi

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

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


