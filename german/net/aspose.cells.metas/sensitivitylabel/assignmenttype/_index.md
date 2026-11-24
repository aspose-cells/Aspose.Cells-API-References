---
title: "SensitivityLabel.AssignmentType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SensitivityLabel-Eigenschaft. Gibt die Zuweisungsmethode für das Sensitivitätslabel zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.metas/sensitivitylabel/assignmenttype/
---
## SensitivityLabel.AssignmentType property

Liest und setzt die Zuweisungsmethode für das Sensitivitätslabel.

```csharp
public SensitivityLabelAssignmentType AssignmentType { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstellen Sie eine Instanz von SensitivityLabel
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Grundlegende Eigenschaften festlegen
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                
                // Demonstrieren Sie das Abrufen des anfänglichen AssignmentType-Werts
                Console.WriteLine("Initial AssignmentType: " + label.AssignmentType);
                
                // Setzen Sie AssignmentType auf Privileged und zeigen Sie die Änderung an
                label.AssignmentType = SensitivityLabelAssignmentType.Privileged;
                Console.WriteLine("After setting Privileged: " + label.AssignmentType);
                
                // Wechseln Sie zurück zu Standard, um zu demonstrieren, dass es les- und schreibbar ist
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                Console.WriteLine("After setting Standard: " + label.AssignmentType);
                
                // Speichere die Arbeitsmappe
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

### Siehe auch

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


