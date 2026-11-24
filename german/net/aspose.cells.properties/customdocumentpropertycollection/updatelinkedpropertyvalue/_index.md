---
title: "CustomDocumentPropertyCollection.UpdateLinkedPropertyValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomDocumentPropertyCollection method. Aktualisiert die Werte aller benutzerdefinierten Eigenschaften, die mit Inhalt verknüpft sind, verwendet den Zellenwert des verknüpften Bereichs, um den Wert der benutzerdefinierten Eigenschaft zu aktualisieren"
type: docs
url: /de/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/
---
## CustomDocumentPropertyCollection.UpdateLinkedPropertyValue method

Aktualisiert die Werte aller benutzerdefinierten Eigenschaften, die mit Inhalt verknüpft sind (Verwenden Sie den Zellenwert des verknüpften Bereichs, um den Wert der benutzerdefinierten Eigenschaft zu aktualisieren).

```csharp
public void UpdateLinkedPropertyValue()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedPropertyValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie einigen Zellen Daten hinzu, die mit benutzerdefinierten Eigenschaften verknüpft werden
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "InitialValue1";
            worksheet.Cells["B1"].Value = "InitialValue2";

            // Verknüpfte benutzerdefinierte Eigenschaften hinzufügen
            workbook.CustomDocumentProperties.AddLinkToContent("CompanyName", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Department", "B1");

            // Zellwerte aktualisieren
            worksheet.Cells["A1"].Value = "UpdatedValue1";
            worksheet.Cells["B1"].Value = "UpdatedValue2";

            // Verknüpfte Eigenschaftswerte aktualisieren
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // Aktualisierte Eigenschaftswerte anzeigen
            Console.WriteLine("CompanyName: " + workbook.CustomDocumentProperties["CompanyName"].Value);
            Console.WriteLine("Department: " + workbook.CustomDocumentProperties["Department"].Value);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


