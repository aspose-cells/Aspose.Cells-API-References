---
title: "WebExtensionPropertyCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WebExtensionPropertyCollection. Rimuove la proprietà per nome"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionpropertycollection/removeat/
---
## WebExtensionPropertyCollection.RemoveAt method

Rimuove la proprietà per nome.

```csharp
public void RemoveAt(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della proprietà. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Creare una raccolta di proprietà web extension
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Aggiungere alcune proprietà alla raccolta
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");
            properties.Add("Property3", "Value3");

            try
            {
                // Chiamare il metodo RemoveAt con parametro string
                properties.RemoveAt("Property2");

                Console.WriteLine("Property with name 'Property2' removed successfully.");
                
                // Visualizzare le proprietà rimanenti
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
            
            // Salva la cartella di lavoro
            workbook.Save("WebExtensionPropertyCollectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


