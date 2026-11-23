---
title: "DocumentPropertyCollection.Remove"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode DocumentPropertyCollection. Supprime une propriété avec le nom spécifié de la collection"
type: docs
url: /fr/net/aspose.cells.properties/documentpropertycollection/remove/
---
## DocumentPropertyCollection.Remove method

Supprime une propriété portant le nom spécifié de la collection.

```csharp
public void Remove(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la propriété, insensible à la casse. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            string inputPath = "example.xlsx";
            string outputPath = "output.xlsm";

            using (FileStream stream = new FileStream(inputPath, FileMode.Open))
            {
                Workbook workbook = new Workbook(stream);
                
                if (workbook.Worksheets.CustomDocumentProperties.Contains("_PID_HLINKS"))
                {
                    workbook.Worksheets.CustomDocumentProperties.Remove("_PID_HLINKS");
                }

                workbook.Save(outputPath, SaveFormat.Xlsm);
            }
        }
    }
}
```

### Voir aussi

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


