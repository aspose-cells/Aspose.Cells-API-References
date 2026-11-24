---
title: "SensitivityLabel.Id"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SensitivityLabel-Eigenschaft. Gibt die Id des SensitivityLabel zurück und legt sie fest."
type: docs
url: /de/net/aspose.cells.metas/sensitivitylabel/id/
---
## SensitivityLabel.Id property

Liest und setzt die ID des Sensitivitätslabels.

```csharp
public string Id { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstellen Sie eine Instanz von SensitivityLabel
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // Demonstrieren Sie das Setzen und Abrufen der Id-Eigenschaft
                string testId = "CONFIDENTIAL_001";
                label.Id = testId;
                
                // Zeigen Sie den Id-Wert an
                Console.WriteLine("Sensitivity Label Id: " + label.Id);
                
                // Ändern Sie den Id-Wert, um zu demonstrieren, dass er les- und schreibbar ist
                label.Id = "INTERNAL_USE_ONLY";
                Console.WriteLine("Updated Sensitivity Label Id: " + label.Id);
                
                // Zeigen Sie, dass die Eigenschaft andere Vorgänge beeinflusst
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

### Siehe auch

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


