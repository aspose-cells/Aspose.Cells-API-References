---
title: "SensitivityLabel.AssignmentType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SensitivityLabel-egenskap. Hämtar och anger tilldelningsmetoden för känslighetsetiketten"
type: docs
url: /sv/net/aspose.cells.metas/sensitivitylabel/assignmenttype/
---
## SensitivityLabel.AssignmentType property

Hämtar och anger tilldelningsmetoden för känslighetsetiketten.

```csharp
public SensitivityLabelAssignmentType AssignmentType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyAssignmentTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en instans av sensitivity label
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Ställ in grundläggande egenskaper
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                
                // Demonstrera hämtning av det initiala AssignmentType-värdet
                Console.WriteLine("Initial AssignmentType: " + label.AssignmentType);
                
                // Ställ in AssignmentType till Privileged och visa förändringen
                label.AssignmentType = SensitivityLabelAssignmentType.Privileged;
                Console.WriteLine("After setting Privileged: " + label.AssignmentType);
                
                // Ändra tillbaka till Standard för att demonstrera att det är läs-skriv
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                Console.WriteLine("After setting Standard: " + label.AssignmentType);
                
                // Spara arbetsboken
                workbook.Save("AssignmentTypeDemo.xlsx");
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

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


