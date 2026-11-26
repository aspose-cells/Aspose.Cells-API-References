---
title: "WorkbookSettings.Compliance"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Указывает версию OOXML для выходного документа. Значение по умолчанию — Ecma376_2006"
type: docs
url: /ru/net/aspose.cells/workbooksettings/compliance/
---
## WorkbookSettings.Compliance property

Указывает версию OOXML для выходного документа. Значение по умолчанию — Ecma376_2006.

```csharp
public OoxmlCompliance Compliance { get; set; }
```

### Примечания

Только для файлов .xlsx.

### Примеры

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
            
            // Установите соответствие в строгий режим
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;
            
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Strict Compliance Demo");
            
            workbook.Save("WorkbookComplianceDemo.xlsx");
        }
    }
}
```

### См. также

* enum [OoxmlCompliance](../../ooxmlcompliance/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


