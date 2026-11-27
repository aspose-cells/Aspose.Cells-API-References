---
title: "WriteProtection.RecommendReadOnly"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WriteProtection-egenskapen. Anger om alternativet Läs-endast rekommenderat är valt"
type: docs
url: /sv/net/aspose.cells/writeprotection/recommendreadonly/
---
## WriteProtection.RecommendReadOnly property

Anger om alternativet Läs endast rekommenderat är valt.

```csharp
public bool RecommendReadOnly { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyRecommendReadOnlyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt kalkylbladet och lägg till lite exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Ställ in RecommendReadOnly till true
            workbook.Settings.WriteProtection.RecommendReadOnly = true;
            
            // Verifiera att egenskapen är inställd
            Console.WriteLine("RecommendReadOnly: " + workbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("IsWriteProtected: " + workbook.Settings.WriteProtection.IsWriteProtected);

            // Spara arbetsboken
            workbook.Save("output_recommend_readonly.xlsx");

            // Läs in den sparade arbetsboken för att verifiera att inställningarna kvarstår
            Workbook loadedWorkbook = new Workbook("output_recommend_readonly.xlsx");
            Console.WriteLine("After loading - RecommendReadOnly: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("After loading - IsWriteProtected: " + loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### Se även

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


