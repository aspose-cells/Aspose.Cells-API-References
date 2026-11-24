---
title: "WriteProtection.RecommendReadOnly"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WriteProtection-Eigenschaft. Gibt an, ob die Option „Read Only Recommended“ ausgewählt ist"
type: docs
url: /de/net/aspose.cells/writeprotection/recommendreadonly/
---
## WriteProtection.RecommendReadOnly property

Gibt an, ob die Option „Read Only Recommended“ ausgewählt ist.

```csharp
public bool RecommendReadOnly { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyRecommendReadOnlyDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das Arbeitsblatt und einige Beispieldaten hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Setze RecommendReadOnly auf true
            workbook.Settings.WriteProtection.RecommendReadOnly = true;
            
            // Überprüfe, ob die Eigenschaft gesetzt ist
            Console.WriteLine("RecommendReadOnly: " + workbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("IsWriteProtected: " + workbook.Settings.WriteProtection.IsWriteProtected);

            // Speichere die Arbeitsmappe
            workbook.Save("output_recommend_readonly.xlsx");

            // Lade die gespeicherte Arbeitsmappe, um zu überprüfen, ob die Einstellungen erhalten bleiben
            Workbook loadedWorkbook = new Workbook("output_recommend_readonly.xlsx");
            Console.WriteLine("After loading - RecommendReadOnly: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("After loading - IsWriteProtected: " + loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### Siehe auch

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


