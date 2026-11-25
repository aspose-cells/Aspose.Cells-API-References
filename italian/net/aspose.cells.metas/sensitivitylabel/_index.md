---
title: "Classe SensitivityLabel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Metas.SensitivityLabel class. Rappresenta l'etichetta di sensibilità"
type: docs
url: /it/net/aspose.cells.metas/sensitivitylabel/
---
## SensitivityLabel class

Rappresenta l'etichetta di sensibilità.

```csharp
public class SensitivityLabel
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AssignmentType](../../aspose.cells.metas/sensitivitylabel/assignmenttype/) { get; set; } | Ottiene e imposta il metodo di assegnazione per l'etichetta di sensibilità. |
| [ContentMarkType](../../aspose.cells.metas/sensitivitylabel/contentmarktype/) { get; set; } | Ottiene e imposta i tipi di marcatura del contenuto che dovrebbero essere applicati a un file. |
| [Id](../../aspose.cells.metas/sensitivitylabel/id/) { get; set; } | Ottiene e imposta l'ID dell'etichetta di sensibilità. |
| [IsEnabled](../../aspose.cells.metas/sensitivitylabel/isenabled/) { get; set; } | Indica se l'etichetta di sensibilità è abilitata |
| [IsRemoved](../../aspose.cells.metas/sensitivitylabel/isremoved/) { get; set; } | Indica se l'etichetta di sensibilità è stata rimossa. |
| [SiteId](../../aspose.cells.metas/sensitivitylabel/siteid/) { get; set; } | Rappresenta l'identificatore del sito Azure Active Directory (Azure AD) corrispondente alla politica dell'etichetta di sensibilità che descrive l'etichetta di sensibilità. |

### Esempi

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
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea un'istanza della classe SensitivityLabel usando la riflessione
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Imposta le proprietà di base
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                label.ContentMarkType = SensitivityLabelMarkType.None;
                
                // Visualizza i valori delle proprietà
                Console.WriteLine($"Sensitivity Label Created:");
                Console.WriteLine($"ID: {label.Id}");
                Console.WriteLine($"Enabled: {label.IsEnabled}");
                Console.WriteLine($"Assignment Type: {label.AssignmentType}");
                Console.WriteLine($"Content Mark Type: {label.ContentMarkType}");
                
                // Salva la cartella di lavoro
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

### Vedi anche

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


