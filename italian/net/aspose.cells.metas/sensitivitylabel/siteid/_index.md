---
title: "SensitivityLabel.SiteId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SensitivityLabel. Rappresenta l'identificatore del sito Azure Active Directory Azure AD corrispondente alla politica di etichetta di sensibilità che descrive l'etichetta di sensibilità"
type: docs
url: /it/net/aspose.cells.metas/sensitivitylabel/siteid/
---
## SensitivityLabel.SiteId property

Rappresenta l'identificatore del sito Azure Active Directory (Azure AD) corrispondente alla politica dell'etichetta di sensibilità che descrive l'etichetta di sensibilità.

```csharp
public string SiteId { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertySiteIdDemo
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

                // Dimostra il recupero del valore iniziale di SiteId
                Console.WriteLine("Initial SiteId: " + label.SiteId);

                // Imposta SiteId su un identificatore di sito Azure AD di esempio
                label.SiteId = "a1b2c3d4-5678-90ef-ghij-klmnopqrstuv";
                Console.WriteLine("After setting SiteId: " + label.SiteId);

                // Modifica SiteId per dimostrare che è leggibile e scrivibile
                label.SiteId = "z9y8x7w6-5432-10uv-wxyz-abcdefghijkl";
                Console.WriteLine("Updated SiteId: " + label.SiteId);

                // Mostra come SiteId si relaziona ad altre proprietà
                Console.WriteLine($"Label {label.Id} with SiteId {label.SiteId} is enabled: {label.IsEnabled}");

                // Salva la cartella di lavoro
                workbook.Save("SiteIdDemo.xlsx");
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


