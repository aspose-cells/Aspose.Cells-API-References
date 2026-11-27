---
title: "Klass SensitivityLabel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Metas.SensitivityLabel klass. Representerar känslighetsetiketten"
type: docs
url: /sv/net/aspose.cells.metas/sensitivitylabel/
---
## SensitivityLabel class

Representerar känslighetsetiketten.

```csharp
public class SensitivityLabel
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AssignmentType](../../aspose.cells.metas/sensitivitylabel/assignmenttype/) { get; set; } | Hämtar och anger tilldelningsmetoden för känslighetsetiketten. |
| [ContentMarkType](../../aspose.cells.metas/sensitivitylabel/contentmarktype/) { get; set; } | Hämtar och anger typerna av innehållsmärkning som ska tillämpas på en fil. |
| [Id](../../aspose.cells.metas/sensitivitylabel/id/) { get; set; } | Hämtar och anger id‑t för känslighetsetiketten. |
| [IsEnabled](../../aspose.cells.metas/sensitivitylabel/isenabled/) { get; set; } | Anger om känslighetsetiketten är aktiverad |
| [IsRemoved](../../aspose.cells.metas/sensitivitylabel/isremoved/) { get; set; } | Anger om känslighetsetiketten har tagits bort. |
| [SiteId](../../aspose.cells.metas/sensitivitylabel/siteid/) { get; set; } | Representerar Azure Active Directory (Azure AD)-platsidentifieraren som motsvarar policyn för känslighetsetikett som beskriver känslighetsetiketten. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class MetasClassSensitivityLabelDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en instans av SensitivityLabel‑klassen med hjälp av reflektion
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Ställ in grundläggande egenskaper
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                label.ContentMarkType = SensitivityLabelMarkType.None;
                
                // Visa egenskapsvärden
                Console.WriteLine($"Sensitivity Label Created:");
                Console.WriteLine($"ID: {label.Id}");
                Console.WriteLine($"Enabled: {label.IsEnabled}");
                Console.WriteLine($"Assignment Type: {label.AssignmentType}");
                Console.WriteLine($"Content Mark Type: {label.ContentMarkType}");
                
                // Spara arbetsboken
                workbook.Save("SensitivityLabelDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SensitivityLabel: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


