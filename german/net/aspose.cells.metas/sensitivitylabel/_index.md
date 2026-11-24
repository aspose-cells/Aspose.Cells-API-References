---
title: "Klasse SensitivityLabel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Metas.SensitivityLabel class. Stellt das Sensitivitätslabel dar."
type: docs
url: /de/net/aspose.cells.metas/sensitivitylabel/
---
## SensitivityLabel class

Stellt das Sensitivitätslabel dar.

```csharp
public class SensitivityLabel
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AssignmentType](../../aspose.cells.metas/sensitivitylabel/assignmenttype/) { get; set; } | Liest und setzt die Zuweisungsmethode für das Sensitivitätslabel. |
| [ContentMarkType](../../aspose.cells.metas/sensitivitylabel/contentmarktype/) { get; set; } | Liest und setzt die Arten der Inhaltskennzeichnung, die auf eine Datei angewendet werden sollen. |
| [Id](../../aspose.cells.metas/sensitivitylabel/id/) { get; set; } | Liest und setzt die ID des Sensitivitätslabels. |
| [IsEnabled](../../aspose.cells.metas/sensitivitylabel/isenabled/) { get; set; } | Gibt an, ob das Sensitivitätslabel aktiviert ist. |
| [IsRemoved](../../aspose.cells.metas/sensitivitylabel/isremoved/) { get; set; } | Gibt an, ob das Sensitivitätslabel entfernt wurde. |
| [SiteId](../../aspose.cells.metas/sensitivitylabel/siteid/) { get; set; } | Stellt die Azure Active Directory (Azure AD)-Site-ID dar, die der Sensitivitätslabel-Richtlinie entspricht, welche das Sensitivitätslabel beschreibt. |

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstellen Sie eine Instanz der SensitivityLabel-Klasse mittels Reflexion.
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Grundlegende Eigenschaften festlegen
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                label.ContentMarkType = SensitivityLabelMarkType.None;
                
                // Eigenschaftswerte anzeigen
                Console.WriteLine($"Sensitivity Label Created:");
                Console.WriteLine($"ID: {label.Id}");
                Console.WriteLine($"Enabled: {label.IsEnabled}");
                Console.WriteLine($"Assignment Type: {label.AssignmentType}");
                Console.WriteLine($"Content Mark Type: {label.ContentMarkType}");
                
                // Speichere die Arbeitsmappe
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

### Siehe auch

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


