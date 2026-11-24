---
title: "SensitivityLabel.IsEnabled"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SensitivityLabel-Eigenschaft. Gibt an, ob das SensitivityLabel aktiviert ist"
type: docs
url: /de/net/aspose.cells.metas/sensitivitylabel/isenabled/
---
## SensitivityLabel.IsEnabled property

Gibt an, ob das Sensitivitätslabel aktiviert ist.

```csharp
public bool IsEnabled { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstellen Sie eine Instanz von SensitivityLabel
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Setzen Sie die Anfangseigenschaften
                label.Id = "CONFIDENTIAL_001";
                
                // Demonstrieren Sie das Abrufen des anfänglichen IsEnabled-Werts
                Console.WriteLine("Initial IsEnabled value: " + label.IsEnabled);
                
                // Setzen Sie IsEnabled auf true und zeigen Sie die Änderung an
                label.IsEnabled = true;
                Console.WriteLine("After enabling: " + label.IsEnabled);
                
                // Schalten Sie den Wert um, um zu zeigen, dass er les- und schreibbar ist
                label.IsEnabled = false;
                Console.WriteLine("After disabling: " + label.IsEnabled);
                
                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


