---
title: "WorkbookSettings.Compliance"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Especifica la versión OOXML para el documento de salida. El valor predeterminado es Ecma376_2006"
type: docs
url: /es/net/aspose.cells/workbooksettings/compliance/
---
## WorkbookSettings.Compliance property

Especifica la versión OOXML para el documento de salida. El valor predeterminado es Ecma376_2006.

```csharp
public OoxmlCompliance Compliance { get; set; }
```

### Observaciones

Solo para archivos .xlsx.

### Ejemplos

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
            
            // Establecer el cumplimiento en modo estricto
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;
            
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Strict Compliance Demo");
            
            workbook.Save("WorkbookComplianceDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [OoxmlCompliance](../../ooxmlcompliance/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


