---
title: "SensitivityLabelCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SensitivityLabelCollection. Aggiunge un'etichetta di sensibilità"
type: docs
url: /it/net/aspose.cells.metas/sensitivitylabelcollection/add/
---
## SensitivityLabelCollection.Add method

Aggiunge un'etichetta di sensibilità.

```csharp
public int Add(string id, bool isEnabled, SensitivityLabelAssignmentType methodType, string siteId, 
    SensitivityLabelMarkType markType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| id | String | L'ID dell'etichetta. |
| isEnabled | Booleano | Indica se questa etichetta di sensibilità è abilitata. |
| methodType | SensitivityLabelAssignmentType | Il tipo di metodo di assegnazione. |
| siteId | String | L'ID del sito. |
| markType | SensitivityLabelMarkType | Il tipo di contrassegno. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelCollectionMethodAddWithStringBooleanSensitivityLabelADemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una nuova SensitivityLabelCollection
            var sensitivityLabels = new SensitivityLabelCollection();
            
            try
            {
                // Chiama il metodo Add con parametri specifici
                int index = sensitivityLabels.Add(
                    id: "Confidential",
                    isEnabled: true,
                    methodType: SensitivityLabelAssignmentType.Privileged,
                    siteId: "Contoso",
                    markType: SensitivityLabelMarkType.Watermark);
                
                Console.WriteLine($"Sensitivity label added at index: {index}");
                
                // Aggiungi alcuni dati per dimostrare l'effetto
                worksheet.Cells["A1"].Value = "Confidential Data";
                worksheet.Cells["A2"].Value = "This document contains sensitive information";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("SensitivityLabelAddDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabelCollection](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


