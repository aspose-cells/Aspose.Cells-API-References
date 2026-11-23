---
title: "CustomXmlPartCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CustomXmlPartCollection. Ajoute un élément à la collection"
type: docs
url: /fr/net/aspose.cells.markup/customxmlpartcollection/add/
---
## CustomXmlPartCollection.Add method

Ajoute un élément à la collection.

```csharp
public int Add(byte[] data, byte[] schemaData)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| données | Byte[] | Le contenu XML de cette partie de stockage de données XML personnalisée. |
| schemaData | Byte[] | Ensemble de schémas XML associés à cette partie XML personnalisée. |

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenir le CustomXmlPartCollection directement à partir du classeur
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // Préparer les données XML et le schéma sous forme de tableaux d'octets
            string xmlData = "<root><item>Test Data</item></root>";
            string schemaData = "<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'><xs:element name='root'><xs:complexType><xs:sequence><xs:element name='item' type='xs:string'/></xs:sequence></xs:complexType></xs:element></xs:schema>";
            
            byte[] xmlBytes = Encoding.UTF8.GetBytes(xmlData);
            byte[] schemaBytes = Encoding.UTF8.GetBytes(schemaData);

            try
            {
                // Appeler la méthode Add avec des paramètres de tableau d'octets
                int index = customXmlParts.Add(xmlBytes, schemaBytes);
                
                Console.WriteLine($"Custom XML part added successfully at index: {index}");
                
                // Enregistrez le classeur pour démontrer l'effet
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

### Voir aussi

* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


