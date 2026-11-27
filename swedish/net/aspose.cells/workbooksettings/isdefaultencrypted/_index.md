---
title: "WorkbookSettings.IsDefaultEncrypted"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Anger om arbetsboken krypteras med standardlösenord om struktur och fönster i arbetsboken är låsta"
type: docs
url: /sv/net/aspose.cells/workbooksettings/isdefaultencrypted/
---
## WorkbookSettings.IsDefaultEncrypted property

Anger om arbetsboken ska krypteras med standardlösenord när struktur och fönster i arbetsboken är låsta.

```csharp
public bool IsDefaultEncrypted { get; set; }
```

### Anmärkningar

Standardvärdet är nu falskt. Det är samma som i MS Excel 2013.

### Exempel

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

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


