---
title: "Protection.AllowEditingScenario"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Schutz-Eigenschaft. Gibt an, ob der Benutzer Szenarien in einem geschützten Arbeitsblatt bearbeiten darf"
type: docs
url: /de/net/aspose.cells/protection/alloweditingscenario/
---
## Protection.AllowEditingScenario property

Stellt dar, ob der Benutzer Szenarien in einem geschützten Arbeitsblatt bearbeiten darf.

```csharp
public bool AllowEditingScenario { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingScenarioDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);

            // Auf die Schutzeinstellungen des Arbeitsblatts zugreifen
            Protection protection = worksheet.Protection;

            // Schutzeigenschaften festlegen, wobei AllowEditingScenario aktiviert ist
            protection.AllowEditingScenario = true;
            protection.AllowFormattingCell = true;  // Corrected property name
            protection.Password = "password123";

            // Schützen Sie das Arbeitsblatt
            worksheet.Protect(ProtectionType.All);

            // Speichere die Arbeitsmappe
            workbook.Save("ProtectionWithScenarioEditing.xlsx");

            Console.WriteLine("Worksheet protected with AllowEditingScenario enabled.");
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


