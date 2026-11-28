---
title: "WorkbookSettings.Compliance"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Çıktı belgesi için OOXML sürümünü belirtir. Varsayılan değer Ecma376_2006'dır"
type: docs
url: /tr/net/aspose.cells/workbooksettings/compliance/
---
## WorkbookSettings.Compliance property

Çıktı belgesi için OOXML sürümünü belirtir. Varsayılan değer Ecma376_2006'dır.

```csharp
public OoxmlCompliance Compliance { get; set; }
```

### Açıklamalar

Yalnızca .xlsx dosyaları için.

### Örnekler

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
            
            // Compliance'ı katı moda ayarlayın
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;
            
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Strict Compliance Demo");
            
            workbook.Save("WorkbookComplianceDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [OoxmlCompliance](../../ooxmlcompliance/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


