---
title: "SensitivityLabel.SiteId"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SensitivityLabel-Eigenschaft. Stellt die Azure Active Directory (Azure AD) Site‑Kennung dar, die der Richtlinie für das Sensitivitätslabel entspricht, welche das Sensitivitätslabel beschreibt."
type: docs
url: /de/net/aspose.cells.metas/sensitivitylabel/siteid/
---
## SensitivityLabel.SiteId property

Stellt die Azure Active Directory (Azure AD)-Site-ID dar, die der Sensitivitätslabel-Richtlinie entspricht, welche das Sensitivitätslabel beschreibt.

```csharp
public string SiteId { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            try
            {
                // Erstellen Sie eine Instanz von SensitivityLabel
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));

                // Grundlegende Eigenschaften festlegen
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;

                // Demonstrieren Sie das Abrufen des anfänglichen SiteId-Werts
                Console.WriteLine("Initial SiteId: " + label.SiteId);

                // Setzen Sie SiteId auf eine Beispiel‑Azure‑AD‑Site‑Kennung
                label.SiteId = "a1b2c3d4-5678-90ef-ghij-klmnopqrstuv";
                Console.WriteLine("After setting SiteId: " + label.SiteId);

                // Ändern Sie SiteId, um zu demonstrieren, dass es les- und schreibbar ist
                label.SiteId = "z9y8x7w6-5432-10uv-wxyz-abcdefghijkl";
                Console.WriteLine("Updated SiteId: " + label.SiteId);

                // Zeigen Sie, wie SiteId zu anderen Eigenschaften in Beziehung steht
                Console.WriteLine($"Label {label.Id} with SiteId {label.SiteId} is enabled: {label.IsEnabled}");

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


