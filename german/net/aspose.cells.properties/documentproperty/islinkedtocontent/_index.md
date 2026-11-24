---
title: "DocumentProperty.IsLinkedToContent"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocumentProperty-Eigenschaft. Gibt an, ob diese Eigenschaft mit dem Inhalt verknüpft ist"
type: docs
url: /de/net/aspose.cells.properties/documentproperty/islinkedtocontent/
---
## DocumentProperty.IsLinkedToContent property

Gibt an, ob diese Eigenschaft mit Inhalt verknüpft ist.

```csharp
public bool IsLinkedToContent { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyIsLinkedToContentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge Beispieldaten zu Zellen hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Company Name";
            worksheet.Cells["B1"].Value = "Company Address";

            // Erstelle verknüpfte benutzerdefinierte Dokumenteigenschaften
            workbook.CustomDocumentProperties.AddLinkToContent("Company", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Address", "B1");

            // Rufe die IsLinkedToContent-Eigenschaft ab und prüfe sie
            DocumentProperty companyProp = workbook.CustomDocumentProperties["Company"];
            Console.WriteLine($"Is 'Company' property linked to content: {companyProp.IsLinkedToContent}");
            Console.WriteLine($"Linked source: {companyProp.Source}");
            Console.WriteLine($"Current value: {companyProp.Value}");

            // Aktualisiere den Zellenwert und aktualisiere verknüpfte Eigenschaften
            worksheet.Cells["A1"].Value = "Updated Company Name";
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // Überprüfe, ob die Eigenschaft aktualisiert wurde
            Console.WriteLine($"Updated value: {companyProp.Value}");

            // Speichere die Arbeitsmappe
            workbook.Save("LinkedPropertiesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


