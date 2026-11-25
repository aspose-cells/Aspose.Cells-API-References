---
title: "ProtectedRange.Password"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ProtectedRange. Rappresenta la password per proteggere l'intervallo"
type: docs
url: /it/net/aspose.cells/protectedrange/password/
---
## ProtectedRange.Password property

Rappresenta la password per proteggere l'intervallo.

```csharp
public string Password { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyPasswordDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea la collezione di intervalli protetti
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // Aggiungi un intervallo protetto
            int index = allowRanges.Add("MyProtectedRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];

            // Imposta la password per l'intervallo protetto
            protectedRange.Password = "12345";

            // Salva la cartella di lavoro
            workbook.Save("ProtectedRangeWithPassword.xlsx");
        }
    }
}
```

### Vedi anche

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


