---
title: "CustomXmlPartCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomXmlPartCollection-Methode. Fügt ein Element zur Sammlung hinzu"
type: docs
url: /de/net/aspose.cells.markup/customxmlpartcollection/add/
---
## CustomXmlPartCollection.Add method

Fügt ein Element zur Sammlung hinzu.

```csharp
public int Add(byte[] data, byte[] schemaData)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Daten | Byte[] | Der XML-Inhalt dieses Custom XML Data Storage Parts. |
| schemaData | Byte[] | Die Menge der XML-Schemas, die mit diesem benutzerdefinierten XML-Teil verknüpft sind. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Rufen Sie die CustomXmlPartCollection direkt aus der Arbeitsmappe ab
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // Bereiten Sie XML-Daten und Schema als Byte-Arrays vor
            string xmlData = "<root><item>Test Data</item></root>";
            string schemaData = "<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'><xs:element name='root'><xs:complexType><xs:sequence><xs:element name='item' type='xs:string'/></xs:sequence></xs:complexType></xs:element></xs:schema>";
            
            byte[] xmlBytes = Encoding.UTF8.GetBytes(xmlData);
            byte[] schemaBytes = Encoding.UTF8.GetBytes(schemaData);

            try
            {
                // Rufen Sie die Add-Methode mit Byte-Array-Parametern auf
                int index = customXmlParts.Add(xmlBytes, schemaBytes);
                
                Console.WriteLine($"Custom XML part added successfully at index: {index}");
                
                // Speichere die Arbeitsmappe, um die Wirkung zu demonstrieren
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

### Siehe auch

* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


