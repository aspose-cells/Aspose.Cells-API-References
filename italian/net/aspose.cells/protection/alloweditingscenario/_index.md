---
title: "Protection.AllowEditingScenario"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta se l'utente è autorizzato a modificare gli scenari su un foglio di lavoro protetto"
type: docs
url: /it/net/aspose.cells/protection/alloweditingscenario/
---
## Protection.AllowEditingScenario property

Rappresenta se all'utente è consentito modificare gli scenari su un foglio di lavoro protetto.

```csharp
public bool AllowEditingScenario { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingScenarioDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);

            // Accedi alle impostazioni di protezione del foglio di lavoro
            Protection protection = worksheet.Protection;

            // Imposta le proprietà di protezione con AllowEditingScenario abilitato
            protection.AllowEditingScenario = true;
            protection.AllowFormattingCell = true;  // Corrected property name
            protection.Password = "password123";

            // Proteggi il foglio di lavoro
            worksheet.Protect(ProtectionType.All);

            // Salva la cartella di lavoro
            workbook.Save("ProtectionWithScenarioEditing.xlsx");

            Console.WriteLine("Worksheet protected with AllowEditingScenario enabled.");
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


