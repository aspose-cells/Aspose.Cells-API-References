---
title: "Protection.AllowEditingContent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta se all\\'utente è consentito modificare il contenuto delle celle bloccate in un foglio di lavoro protetto"
type: docs
url: /it/net/aspose.cells/protection/alloweditingcontent/
---
## Protection.AllowEditingContent property

Rappresenta se all'utente è consentito modificare il contenuto delle celle bloccate su un foglio di lavoro protetto.

```csharp
public bool AllowEditingContent { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingContentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Proteggi il foglio di lavoro con una password
            worksheet.Protect(ProtectionType.All, "password", null);
            
            // Controlla e visualizza la proprietà AllowEditingContent
            Console.WriteLine("AllowEditingContent before setting: " + worksheet.Protection.AllowEditingContent);
            
            // Modifica la proprietà AllowEditingContent
            worksheet.Protection.AllowEditingContent = true;
            
            // Controlla e visualizza la proprietà aggiornata
            Console.WriteLine("AllowEditingContent after setting: " + worksheet.Protection.AllowEditingContent);
            
            // Salva la cartella di lavoro
            workbook.Save("ProtectionPropertyAllowEditingContentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


