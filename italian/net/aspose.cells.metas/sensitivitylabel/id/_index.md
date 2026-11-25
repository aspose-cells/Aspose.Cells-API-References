---
title: "SensitivityLabel.Id"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SensitivityLabel. Ottiene e imposta l'ID dell'etichetta di sensibilità"
type: docs
url: /it/net/aspose.cells.metas/sensitivitylabel/id/
---
## SensitivityLabel.Id property

Ottiene e imposta l'ID dell'etichetta di sensibilità.

```csharp
public string Id { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Creare un'istanza di SensitivityLabel
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // Dimostrare l'impostazione e il recupero della proprietà Id
                string testId = "CONFIDENTIAL_001";
                label.Id = testId;
                
                // Visualizzare il valore dell'ID
                Console.WriteLine("Sensitivity Label Id: " + label.Id);
                
                // Modifica il valore Id per dimostrare che è leggibile e scrivibile
                label.Id = "INTERNAL_USE_ONLY";
                Console.WriteLine("Updated Sensitivity Label Id: " + label.Id);
                
                // Mostra che la proprietà influisce su altre operazioni
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

### Vedi anche

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


