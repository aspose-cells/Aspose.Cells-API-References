---
title: "SensitivityLabel.IsRemoved"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SensitivityLabel‑egenskapen. Anger om sensitivity label har tagits bort"
type: docs
url: /sv/net/aspose.cells.metas/sensitivitylabel/isremoved/
---
## SensitivityLabel.IsRemoved property

Anger om känslighetsetiketten har tagits bort.

```csharp
public bool IsRemoved { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIsRemovedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en sensitivity label‑instans via reflektion
                // eftersom direkt instansiering inte är tillgänglig
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // Ange nödvändiga egenskaper
                label.Id = "SENSITIVE_DATA";
                label.IsEnabled = true;
                label.IsRemoved = false;
                
                // Visa initialt IsRemoved‑värde
                Console.WriteLine("Initial IsRemoved value: " + label.IsRemoved);
                
                // Demonstrera att sätta IsRemoved‑egenskapen (eftersom den är läslig/skrivbar)
                label.IsRemoved = true;
                Console.WriteLine("After setting IsRemoved: " + label.IsRemoved);
                
                // Växla värdet tillbaka för att visa att det kan ändras
                label.IsRemoved = false;
                Console.WriteLine("Final IsRemoved value: " + label.IsRemoved);
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


