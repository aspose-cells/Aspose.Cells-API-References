---
title: "SensitivityLabel.IsRemoved"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SensitivityLabel-Eigenschaft. Gibt an, ob das SensitivityLabel entfernt wurde"
type: docs
url: /de/net/aspose.cells.metas/sensitivitylabel/isremoved/
---
## SensitivityLabel.IsRemoved property

Gibt an, ob das Sensitivitätslabel entfernt wurde.

```csharp
public bool IsRemoved { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstellen Sie eine SensitivityLabel-Instanz mittels Reflexion
                // da eine direkte Instanziierung nicht verfügbar ist
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // Setzen Sie die erforderlichen Eigenschaften
                label.Id = "SENSITIVE_DATA";
                label.IsEnabled = true;
                label.IsRemoved = false;
                
                // Zeigen Sie den anfänglichen IsRemoved-Wert an
                Console.WriteLine("Initial IsRemoved value: " + label.IsRemoved);
                
                // Demonstrieren Sie das Setzen der IsRemoved-Eigenschaft (da sie les- und schreibbar ist)
                label.IsRemoved = true;
                Console.WriteLine("After setting IsRemoved: " + label.IsRemoved);
                
                // Schalten Sie den Wert zurück, um zu zeigen, dass er geändert werden kann
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

### Siehe auch

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


