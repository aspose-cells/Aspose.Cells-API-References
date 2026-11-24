---
title: "DocumentPropertyCollection.RemoveAt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocumentPropertyCollection-Methode. Entfernt eine Eigenschaft am angegebenen Index"
type: docs
url: /de/net/aspose.cells.properties/documentpropertycollection/removeat/
---
## DocumentPropertyCollection.RemoveAt method

Entfernt eine Eigenschaft am angegebenen Index.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der nullbasierte Index. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf benutzerdefinierte Dokumenteigenschaften zu (statt der integrierten)
            DocumentPropertyCollection properties = workbook.Worksheets.CustomDocumentProperties;
            
            // Fügen Sie einige benutzerdefinierte Eigenschaften hinzu, um das Entfernen zu demonstrieren
            ((CustomDocumentPropertyCollection)properties).Add("Property1", "Value1");
            ((CustomDocumentPropertyCollection)properties).Add("Property2", "Value2");
            ((CustomDocumentPropertyCollection)properties).Add("Property3", "Value3");

            try
            {
                // Zeigen Sie die Eigenschaften vor dem Entfernen an
                Console.WriteLine("Properties before removal:");
                foreach (DocumentProperty prop in properties)
                {
                    Console.WriteLine($"{prop.Name}: {prop.Value}");
                }

                // Rufen Sie RemoveAt mit Index 1 (zweite Eigenschaft) auf
                properties.RemoveAt(1);

                // Eigenschaften nach dem Entfernen anzeigen
                Console.WriteLine("\nProperties after removal:");
                foreach (DocumentProperty prop in properties)
                {
                    Console.WriteLine($"{prop.Name}: {prop.Value}");
                }

                Console.WriteLine("RemoveAt method executed successfully with parameter (Int32)");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Error: Index out of range. {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("RemoveAtMethodDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


