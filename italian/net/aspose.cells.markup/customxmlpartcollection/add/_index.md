---
title: "CustomXmlPartCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CustomXmlPartCollection. Aggiunge un elemento alla collezione"
type: docs
url: /it/net/aspose.cells.markup/customxmlpartcollection/add/
---
## CustomXmlPartCollection.Add method

Aggiunge un elemento alla collezione.

```csharp
public int Add(byte[] data, byte[] schemaData)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dati | Byte[] | Il contenuto XML di questa parte di archiviazione dati XML personalizzata. |
| schemaData | Byte[] | L'insieme di schemi XML associati a questa parte XML personalizzata. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;
    using System.Text;

    public class CustomXmlPartCollectionMethodAddWithByteByteDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Ottieni CustomXmlPartCollection direttamente dal workbook
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // Prepara i dati XML e lo schema come array di byte
            string xmlData = "<root><item>Test Data</item></root>";
            string schemaData = "<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'><xs:element name='root'><xs:complexType><xs:sequence><xs:element name='item' type='xs:string'/></xs:sequence></xs:complexType></xs:element></xs:schema>";
            
            byte[] xmlBytes = Encoding.UTF8.GetBytes(xmlData);
            byte[] schemaBytes = Encoding.UTF8.GetBytes(schemaData);

            try
            {
                // Chiama il metodo Add con parametri array di byte
                int index = customXmlParts.Add(xmlBytes, schemaBytes);
                
                Console.WriteLine($"Custom XML part added successfully at index: {index}");
                
                // Salva la cartella di lavoro per dimostrare l'effetto
                workbook.Save("CustomXmlPartAddDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding custom XML part: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


