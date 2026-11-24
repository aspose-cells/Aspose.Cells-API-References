---
title: "WorkbookSettings.Compliance"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt die OOXML-Version für das Ausgabedokument an. Der Standardwert ist Ecma376_2006."
type: docs
url: /de/net/aspose.cells/workbooksettings/compliance/
---
## WorkbookSettings.Compliance property

Gibt die OOXML-Version für das Ausgabedokument an. Der Standardwert ist Ecma376_2006.

```csharp
public OoxmlCompliance Compliance { get; set; }
```

### Hinweise

Nur für .xlsx-Dateien.

### Beispiele

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
            
            // Setzen Sie compliance auf den strikten Modus.
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;
            
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Strict Compliance Demo");
            
            workbook.Save("WorkbookComplianceDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [OoxmlCompliance](../../ooxmlcompliance/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


