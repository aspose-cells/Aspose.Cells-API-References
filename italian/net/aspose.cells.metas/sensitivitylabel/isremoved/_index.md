---
title: "SensitivityLabel.IsRemoved"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SensitivityLabel. Indica se l'etichetta di sensibilità è stata rimossa"
type: docs
url: /it/net/aspose.cells.metas/sensitivitylabel/isremoved/
---
## SensitivityLabel.IsRemoved property

Indica se l'etichetta di sensibilità è stata rimossa.

```csharp
public bool IsRemoved { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea un'istanza di etichetta di sensibilità tramite reflection
                // poiché l'instanziazione diretta non è disponibile
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // Imposta le proprietà richieste
                label.Id = "SENSITIVE_DATA";
                label.IsEnabled = true;
                label.IsRemoved = false;
                
                // Visualizza il valore iniziale di IsRemoved
                Console.WriteLine("Initial IsRemoved value: " + label.IsRemoved);
                
                // Dimostra l'impostazione della proprietà IsRemoved (poiché è leggibile e scrivibile)
                label.IsRemoved = true;
                Console.WriteLine("After setting IsRemoved: " + label.IsRemoved);
                
                // Alterna il valore nuovamente per mostrare che può essere modificato
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

### Vedi anche

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


