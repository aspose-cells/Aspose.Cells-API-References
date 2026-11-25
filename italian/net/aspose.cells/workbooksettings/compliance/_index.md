---
title: "WorkbookSettings.Compliance"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Specifica la versione OOXML per il documento di output. Il valore predefinito è Ecma376_2006"
type: docs
url: /it/net/aspose.cells/workbooksettings/compliance/
---
## WorkbookSettings.Compliance property

Specifica la versione OOXML per il documento di output. Il valore predefinito è Ecma376_2006.

```csharp
public OoxmlCompliance Compliance { get; set; }
```

### Osservazioni

Solo per file .xlsx.

### Esempi

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
            
            // Impostare la conformità in modalità rigorosa
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;
            
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Strict Compliance Demo");
            
            workbook.Save("WorkbookComplianceDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [OoxmlCompliance](../../ooxmlcompliance/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


