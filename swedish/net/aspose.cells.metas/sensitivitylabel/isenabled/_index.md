---
title: "SensitivityLabel.IsEnabled"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SensitivityLabel-egenskap. Anger om känslighetsetiketten är aktiverad"
type: docs
url: /sv/net/aspose.cells.metas/sensitivitylabel/isenabled/
---
## SensitivityLabel.IsEnabled property

Anger om känslighetsetiketten är aktiverad

```csharp
public bool IsEnabled { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIsEnabledDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en instans av sensitivity label
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Ställ in initiala egenskaper
                label.Id = "CONFIDENTIAL_001";
                
                // Demonstrera hämtning av det initiala IsEnabled-värdet
                Console.WriteLine("Initial IsEnabled value: " + label.IsEnabled);
                
                // Ställ in IsEnabled till true och visa förändringen
                label.IsEnabled = true;
                Console.WriteLine("After enabling: " + label.IsEnabled);
                
                // Växla värdet för att demonstrera att det är läs-skriv
                label.IsEnabled = false;
                Console.WriteLine("After disabling: " + label.IsEnabled);
                
                // Spara arbetsboken
                workbook.Save("IsEnabledDemo.xlsx");
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


