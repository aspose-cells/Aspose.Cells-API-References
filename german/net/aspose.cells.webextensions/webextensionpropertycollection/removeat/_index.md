---
title: "WebExtensionPropertyCollection.RemoveAt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionPropertyCollection-Methode. Entfernt die Eigenschaft anhand des Namens"
type: docs
url: /de/net/aspose.cells.webextensions/webextensionpropertycollection/removeat/
---
## WebExtensionPropertyCollection.RemoveAt method

Entfernt die Eigenschaft anhand des Namens.

```csharp
public void RemoveAt(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Eigenschaft. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine WebExtension-Eigenschaftssammlung
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Füge einige Eigenschaften zur Sammlung hinzu
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");
            properties.Add("Property3", "Value3");

            try
            {
                // Rufe die RemoveAt-Methode mit einem String-Parameter auf
                properties.RemoveAt("Property2");

                Console.WriteLine("Property with name 'Property2' removed successfully.");
                
                // Zeige die verbleibenden Eigenschaften an
                Console.WriteLine("Remaining properties:");
                for (int i = 0; i < properties.Count; i++)
                {
                    Console.WriteLine($"{properties[i].Name}: {properties[i].Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("WebExtensionPropertyCollectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


