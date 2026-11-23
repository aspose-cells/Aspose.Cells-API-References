---
title: "ListObject.Resize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ListObject. Redimensionner la plage de l'objet de liste"
type: docs
url: /fr/net/aspose.cells.tables/listobject/resize/
---
## ListObject.Resize method

Redimensionne la plage de l'objet de liste.

```csharp
public void Resize(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | L'index de ligne de départ de la nouvelle plage. |
| startColumn | Int32 | L'index de colonne de départ de la nouvelle plage. |
| endRow | Int32 | L'index de ligne de fin de la nouvelle plage. |
| endColumn | Int32 | L'index de colonne de fin de la nouvelle plage. |
| hasHeaders | Boolean | Indique si ce tableau possède des en-têtes. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodResizeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue("Item " + (i + 1));
                worksheet.Cells[i, 1].PutValue(i * 10);
            }

            // Créer un objet de liste
            int index = worksheet.ListObjects.Add(0, 0, 5, 1, true);
            ListObject listObj = worksheet.ListObjects[index];
            listObj.TableStyleType = TableStyleType.TableStyleLight2;

            // Redimensionner l'objet de liste
            listObj.Resize(0, 0, 9, 1, true);

            // Enregistrez le classeur
            workbook.Save("ResizedListObject.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


