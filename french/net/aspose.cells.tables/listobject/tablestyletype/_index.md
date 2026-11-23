---
title: "ListObject.TableStyleType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListObject. Obtient le style de tableau intégré"
type: docs
url: /fr/net/aspose.cells.tables/listobject/tablestyletype/
---
## ListObject.TableStyleType property

Obtient et le style de tableau intégré.

```csharp
public TableStyleType TableStyleType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyTableStyleTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i+1}-{j+1}");
                }
            }
            
            // Obtenir la collection d'objets de liste
            ListObjectCollection tables = worksheet.ListObjects;
            
            // Ajouter un tableau
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[0];
            
            // Définir le style du tableau
            table.TableStyleType = TableStyleType.TableStyleDark2;
            
            // Enregistrez le classeur
            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TableStyleType](../../tablestyletype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


