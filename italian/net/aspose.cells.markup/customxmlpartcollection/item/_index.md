---
title: "CustomXmlPartCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CustomXmlPartCollection. Ottiene un elemento all'indice specificato"
type: docs
url: /it/net/aspose.cells.markup/customxmlpartcollection/item/
---
## CustomXmlPartCollection indexer

Ottiene un elemento all'indice specificato.

```csharp
public CustomXmlPart this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class CustomXmlPartCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi a CustomXmlPartCollection direttamente dal Workbook
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // Dati XML di esempio
            string xmlData = "<root><item>Test Data</item></root>";
            byte[] xmlBytes = System.Text.Encoding.UTF8.GetBytes(xmlData);
            
            // Aggiungi una parte XML personalizzata
            int index = customXmlParts.Add(xmlBytes, null);
            
            // Accedi all'elemento utilizzando la proprietà Item
            CustomXmlPart part = customXmlParts[index];
            
            // Visualizza l'ID della parte XML personalizzata
            Console.WriteLine("Custom XML Part ID: " + part.ID);
            
            // Recupera i dati XML dalla parte
            string retrievedXml = System.Text.Encoding.UTF8.GetString(part.Data);
            Console.WriteLine("XML Content: " + retrievedXml);
            
            // Salva la cartella di lavoro
            workbook.Save("CustomXmlPartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CustomXmlPart](../../customxmlpart/)
* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


