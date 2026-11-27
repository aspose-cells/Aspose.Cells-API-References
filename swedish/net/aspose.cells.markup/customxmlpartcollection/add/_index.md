---
title: "CustomXmlPartCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomXmlPartCollection metod. Lägger till ett objekt i samlingen"
type: docs
url: /sv/net/aspose.cells.markup/customxmlpartcollection/add/
---
## CustomXmlPartCollection.Add method

Lägger till ett objekt i samlingen.

```csharp
public int Add(byte[] data, byte[] schemaData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| data | Byte[] | XML-innehållet för denna Custom XML Data Storage Part. |
| schemaData | Byte[] | Mängden XML-scheman som är associerade med denna anpassade XML-del. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta CustomXmlPartCollection direkt från workbook
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // Förbered XML-data och schema som byte-arrayer
            string xmlData = "<root><item>Test Data</item></root>";
            string schemaData = "<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'><xs:element name='root'><xs:complexType><xs:sequence><xs:element name='item' type='xs:string'/></xs:sequence></xs:complexType></xs:element></xs:schema>";
            
            byte[] xmlBytes = Encoding.UTF8.GetBytes(xmlData);
            byte[] schemaBytes = Encoding.UTF8.GetBytes(schemaData);

            try
            {
                // Anropa Add-metoden med byte-arrayparametrar
                int index = customXmlParts.Add(xmlBytes, schemaBytes);
                
                Console.WriteLine($"Custom XML part added successfully at index: {index}");
                
                // Spara arbetsboken för att demonstrera effekten
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

### Se även

* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


