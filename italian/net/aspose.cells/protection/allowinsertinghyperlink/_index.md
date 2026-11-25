---
title: "Protection.AllowInsertingHyperlink"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta se l'inserimento di collegamenti ipertestuali è consentito su un foglio di lavoro protetto"
type: docs
url: /it/net/aspose.cells/protection/allowinsertinghyperlink/
---
## Protection.AllowInsertingHyperlink property

Rappresenta se l'inserimento dei collegamenti ipertestuali è consentito su un foglio di lavoro protetto

```csharp
public bool AllowInsertingHyperlink { get; set; }
```

### Esempi

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

            // Aggiungi un collegamento ipertestuale per dimostrare la funzionalità
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            workbook.Save("AllowInsertingHyperlinkDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


