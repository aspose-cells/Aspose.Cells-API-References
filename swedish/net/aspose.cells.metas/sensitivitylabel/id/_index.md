---
title: "SensitivityLabel.Id"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SensitivityLabel‑egenskapen. Hämtar och anger id‑t för sensitivity label"
type: docs
url: /sv/net/aspose.cells.metas/sensitivitylabel/id/
---
## SensitivityLabel.Id property

Hämtar och anger id‑t för känslighetsetiketten.

```csharp
public string Id { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIdDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en instans av sensitivity label
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // Demonstrera att sätta och hämta Id‑egenskapen
                string testId = "CONFIDENTIAL_001";
                label.Id = testId;
                
                // Visa Id‑värdet
                Console.WriteLine("Sensitivity Label Id: " + label.Id);
                
                // Ändra Id‑värdet för att demonstrera att det är läsligt/skrivbart
                label.Id = "INTERNAL_USE_ONLY";
                Console.WriteLine("Updated Sensitivity Label Id: " + label.Id);
                
                // Visa att egenskapen påverkar andra operationer
                label.IsEnabled = true;
                Console.WriteLine($"Label {label.Id} is enabled: {label.IsEnabled}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


