---
title: "SensitivityLabel.SiteId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SensitivityLabel-egenskap. Representerar Azure Active Directory Azure AD-platsidentifieraren som motsvarar känslighetsetikettpolicyn som beskriver känslighetsetiketten"
type: docs
url: /sv/net/aspose.cells.metas/sensitivitylabel/siteid/
---
## SensitivityLabel.SiteId property

Representerar Azure Active Directory (Azure AD)-platsidentifieraren som motsvarar policyn för känslighetsetikett som beskriver känslighetsetiketten.

```csharp
public string SiteId { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Skapa en instans av sensitivity label
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));

                // Ställ in grundläggande egenskaper
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;

                // Demonstrera hämtning av det initiala SiteId-värdet
                Console.WriteLine("Initial SiteId: " + label.SiteId);

                // Ställ in SiteId till ett exempel på en Azure AD-platsidentifierare
                label.SiteId = "a1b2c3d4-5678-90ef-ghij-klmnopqrstuv";
                Console.WriteLine("After setting SiteId: " + label.SiteId);

                // Ändra SiteId för att demonstrera att det är läs-skriv
                label.SiteId = "z9y8x7w6-5432-10uv-wxyz-abcdefghijkl";
                Console.WriteLine("Updated SiteId: " + label.SiteId);

                // Visa hur SiteId relaterar till andra egenskaper
                Console.WriteLine($"Label {label.Id} with SiteId {label.SiteId} is enabled: {label.IsEnabled}");

                // Spara arbetsboken
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

### Se även

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


