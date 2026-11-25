---
title: "SensitivityLabel.IsEnabled"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SensitivityLabel. Indica se l'etichetta di sensibilità è abilitata"
type: docs
url: /it/net/aspose.cells.metas/sensitivitylabel/isenabled/
---
## SensitivityLabel.IsEnabled property

Indica se l'etichetta di sensibilità è abilitata

```csharp
public bool IsEnabled { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Creare un'istanza di SensitivityLabel
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Imposta le proprietà iniziali
                label.Id = "CONFIDENTIAL_001";
                
                // Dimostra il recupero del valore iniziale di IsEnabled
                Console.WriteLine("Initial IsEnabled value: " + label.IsEnabled);
                
                // Imposta IsEnabled su true e visualizza la modifica
                label.IsEnabled = true;
                Console.WriteLine("After enabling: " + label.IsEnabled);
                
                // Alterna il valore per dimostrare che è leggibile e scrivibile
                label.IsEnabled = false;
                Console.WriteLine("After disabling: " + label.IsEnabled);
                
                // Salva la cartella di lavoro
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

### Vedi anche

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


