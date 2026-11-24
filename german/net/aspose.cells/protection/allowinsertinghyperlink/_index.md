---
title: "Protection.AllowInsertingHyperlink"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Protection-Eigenschaft. Gibt an, ob das Einfügen von Hyperlinks in einem geschützten Arbeitsblatt erlaubt ist."
type: docs
url: /de/net/aspose.cells/protection/allowinsertinghyperlink/
---
## Protection.AllowInsertingHyperlink property

Stellt dar, ob das Einfügen von Hyperlinks in einem geschützten Arbeitsblatt erlaubt ist

```csharp
public bool AllowInsertingHyperlink { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingHyperlinkDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Protection protection = worksheet.Protection;
            protection.AllowInsertingHyperlink = true;
            protection.Password = "password123";

            // Füge einen Hyperlink hinzu, um die Funktionalität zu demonstrieren
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            workbook.Save("AllowInsertingHyperlinkDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


