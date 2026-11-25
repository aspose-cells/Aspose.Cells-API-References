---
title: "DocumentPropertyCollection.IndexOf"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DocumentPropertyCollection. Ottiene l'indice di una proprietà per nome"
type: docs
url: /it/net/aspose.cells.properties/documentpropertycollection/indexof/
---
## DocumentPropertyCollection.IndexOf method

Ottiene l'indice di una proprietà per nome.

```csharp
public int IndexOf(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della proprietà, senza distinzione tra maiuscole e minuscole. |

### Valore di ritorno

L'indice basato su zero. Valore negativo se non trovato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyCollectionMethodIndexOfWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Ottieni la collezione delle proprietà del documento predefinite
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;

            // Per le proprietà predefinite, possiamo impostare solo i valori delle proprietà esistenti
            // Per aggiungere proprietà personalizzate, dovremmo usare CustomDocumentPropertyCollection
            // Qui imposteremo solo alcune proprietà predefinite esistenti per dimostrazione
            properties["Title"].Value = "Value1";
            properties["Subject"].Value = "Value2";
            properties["Author"].Value = "Value3";

            try
            {
                // Chiama il metodo IndexOf con parametro stringa
                int index = properties.IndexOf("Subject");
                
                // Visualizza il risultato
                Console.WriteLine($"Index of 'Subject': {index}");
                
                // Mostra la proprietà all'indice trovato
                if (index >= 0)
                {
                    DocumentProperty property = properties[index];
                    Console.WriteLine($"Property at index {index}: {property.Name} = {property.Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IndexOf method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("DocumentPropertyIndexOfDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


