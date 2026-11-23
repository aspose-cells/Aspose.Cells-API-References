---
title: "Classe CustomXmlPart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Markup.CustomXmlPart classe. Représente une partie de stockage de données XML personnalisée (Custom XML Data Storage Part) contenant des données XML personnalisées dans un package"
type: docs
url: /fr/net/aspose.cells.markup/customxmlpart/
---
## CustomXmlPart class

Représente une partie de stockage de données XML personnalisées (données XML personnalisées dans un package).

```csharp
public class CustomXmlPart
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Data](../../aspose.cells.markup/customxmlpart/data/) { get; set; } | Obtient ou définit le contenu XML de cette Custom XML Data Storage Part. |
| [ID](../../aspose.cells.markup/customxmlpart/id/) { get; set; } | Obtient et définit l'ID du custom xml part. |
| [SchemaData](../../aspose.cells.markup/customxmlpart/schemadata/) { get; set; } | Obtient et définit le contenu XML de cette Custom XML Schema Data Storage Part. |

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class MarkupClassCustomXmlPartDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomXmlPartCollection xmlParts = workbook.CustomXmlParts;

            string xmlData = "<root><item>Sample Data</item></root>";
            byte[] dataBytes = Encoding.UTF8.GetBytes(xmlData);

            string originalId = Guid.NewGuid().ToString();
            int index = xmlParts.Add(dataBytes, null);
            CustomXmlPart newPart = xmlParts[index];
            newPart.ID = originalId;

            Console.WriteLine("Original ID: " + originalId);
            Console.WriteLine("Stored ID: " + newPart.ID);

            string newId = Guid.NewGuid().ToString();
            newPart.ID = newId;
            Console.WriteLine("Updated ID: " + newId);

            workbook.Save("output.xlsx");

            Workbook loadedWorkbook = new Workbook("output.xlsx");
            CustomXmlPart retrievedPart = loadedWorkbook.CustomXmlParts.SelectByID(newId);
            Console.WriteLine("Retrieved ID: " + (retrievedPart != null ? retrievedPart.ID : "Not found"));
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


