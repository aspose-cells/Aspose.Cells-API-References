---
title: "WorkbookSettings.Compliance"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Anger OOXML-versionen för utdokumentet. Standardvärdet är Ecma376_2006"
type: docs
url: /sv/net/aspose.cells/workbooksettings/compliance/
---
## WorkbookSettings.Compliance property

Anger OOXML-versionen för utdokumentet. Standardvärdet är Ecma376_2006.

```csharp
public OoxmlCompliance Compliance { get; set; }
```

### Anmärkningar

Endast för .xlsx-filer.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyComplianceDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WorkbookSettings settings = workbook.Settings;
            
            // Ställ in compliance till strikt läge
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;
            
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Strict Compliance Demo");
            
            workbook.Save("WorkbookComplianceDemo.xlsx");
        }
    }
}
```

### Se även

* enum [OoxmlCompliance](../../ooxmlcompliance/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


