---
title: "SensitivityLabel.AssignmentType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SensitivityLabel. Ottiene e imposta il metodo di assegnazione per l'etichetta di sensibilità"
type: docs
url: /it/net/aspose.cells.metas/sensitivitylabel/assignmenttype/
---
## SensitivityLabel.AssignmentType property

Ottiene e imposta il metodo di assegnazione per l'etichetta di sensibilità.

```csharp
public SensitivityLabelAssignmentType AssignmentType { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Creare un'istanza di SensitivityLabel
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Imposta le proprietà di base
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                
                // Dimostra il recupero del valore iniziale di AssignmentType
                Console.WriteLine("Initial AssignmentType: " + label.AssignmentType);
                
                // Imposta AssignmentType su Privileged e visualizza la modifica
                label.AssignmentType = SensitivityLabelAssignmentType.Privileged;
                Console.WriteLine("After setting Privileged: " + label.AssignmentType);
                
                // Ripristina a Standard per dimostrare che è in lettura-scrittura
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                Console.WriteLine("After setting Standard: " + label.AssignmentType);
                
                // Salva la cartella di lavoro
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

### Vedi anche

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


