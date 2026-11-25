---
title: "DocumentPropertyCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DocumentPropertyCollection. Rimuove una proprietà all'indice specificato"
type: docs
url: /it/net/aspose.cells.properties/documentpropertycollection/removeat/
---
## DocumentPropertyCollection.RemoveAt method

Rimuove una proprietà all'indice specificato.

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice basato su zero. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle proprietà documento personalizzate (invece di quelle integrate)
            DocumentPropertyCollection properties = workbook.Worksheets.CustomDocumentProperties;
            
            // Aggiungi alcune proprietà personalizzate per dimostrare la rimozione
            ((CustomDocumentPropertyCollection)properties).Add("Property1", "Value1");
            ((CustomDocumentPropertyCollection)properties).Add("Property2", "Value2");
            ((CustomDocumentPropertyCollection)properties).Add("Property3", "Value3");

            try
            {
                // Visualizza le proprietà prima della rimozione
                Console.WriteLine("Properties before removal:");
                foreach (DocumentProperty prop in properties)
                {
                    Console.WriteLine($"{prop.Name}: {prop.Value}");
                }

                // Chiama RemoveAt con indice 1 (seconda proprietà)
                properties.RemoveAt(1);

                // Visualizza le proprietà dopo la rimozione
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
            
            // Salva la cartella di lavoro
            workbook.Save("RemoveAtMethodDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


