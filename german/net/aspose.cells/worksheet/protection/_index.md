---
title: "Worksheet.Protection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Stellt die verschiedenen Schutzoptionen dar, die für ein Arbeitsblatt verfügbar sind. Unterstützt erweiterte Schutzoptionen in ExcelXP und höheren Versionen"
type: docs
url: /de/net/aspose.cells/worksheet/protection/
---
## Worksheet.Protection property

Stellt die verschiedenen Arten von Schutzoptionen dar, die für ein Arbeitsblatt verfügbar sind. Unterstützt erweiterte Schutzoptionen in ExcelXP und höheren Versionen.

```csharp
public Protection Protection { get; }
```

### Hinweise

Diese Eigenschaft kann das Arbeitsblatt in allen Excel-Dateiversionen schützen und unterstützt erweiterte Schutzoptionen in ExcelXP und höheren Versionen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyProtectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Schutzeigenschaften zugreifen
            Protection protection = sheet.Protection;
            
            // Schutzeigenschaften festlegen
            protection.AllowEditingObject = false;
            protection.AllowEditingScenario = false;
            
            // Arbeitsblatt schützen (die Protect-Methode verwenden, anstatt IsProtectedWithPassword direkt zu setzen)
            sheet.Protect(ProtectionType.All, "password123", null);

            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetProtectionDemo.xlsx");

            // Schutzeinstellungen überprüfen
            Console.WriteLine("AllowEditingObject: " + protection.AllowEditingObject);
            Console.WriteLine("AllowEditingScenario: " + protection.AllowEditingScenario);
        }
    }
}
```

### Siehe auch

* class [Protection](../../protection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


