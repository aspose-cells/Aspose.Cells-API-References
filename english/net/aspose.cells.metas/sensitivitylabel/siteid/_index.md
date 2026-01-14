---
title: SensitivityLabel.SiteId
second_title: Aspose.Cells for .NET API Reference
description: SensitivityLabel property. Represents the Azure Active Directory Azure AD site identifier corresponding to the sensitivity label policy which describes the sensitivity label
type: docs
url: /net/aspose.cells.metas/sensitivitylabel/siteid/
---
## SensitivityLabel.SiteId property

Represents the Azure Active Directory (Azure AD) site identifier corresponding to the sensitivity label policy which describes the sensitivity label.

```csharp
public string SiteId { get; set; }
```

### Examples

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
            // Create a new workbook
            Workbook workbook = new Workbook();

            try
            {
                // Create a sensitivity label instance
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));

                // Set basic properties
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;

                // Demonstrate getting the initial SiteId value
                Console.WriteLine("Initial SiteId: " + label.SiteId);

                // Set SiteId to a sample Azure AD site identifier
                label.SiteId = "a1b2c3d4-5678-90ef-ghij-klmnopqrstuv";
                Console.WriteLine("After setting SiteId: " + label.SiteId);

                // Change SiteId to demonstrate it's read-write
                label.SiteId = "z9y8x7w6-5432-10uv-wxyz-abcdefghijkl";
                Console.WriteLine("Updated SiteId: " + label.SiteId);

                // Show how SiteId relates to other properties
                Console.WriteLine($"Label {label.Id} with SiteId {label.SiteId} is enabled: {label.IsEnabled}");

                // Save the workbook
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

### See Also

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


