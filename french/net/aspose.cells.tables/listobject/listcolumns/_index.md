---
title: "ListObject.ListColumns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListObject. Obtient la liste ListColumn de ce tableau"
type: docs
url: /fr/net/aspose.cells.tables/listobject/listcolumns/
---
## ListObject.ListColumns property

Obtient la liste [`ListColumn`](../../listcolumn/) de ce tableau.

```csharp
public ListColumnCollection ListColumns { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyListColumnsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
                }
            }

            // Créer un objet de liste
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add(0, 0, 9, 4, true);
            ListObject listObject = listObjects[index];
            
            // Activer les totaux et définir le calcul pour la 5e colonne
            listObject.ShowTotals = true;
            listObject.ListColumns[4].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
            
            // Appliquer le style du tableau
            listObject.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleLight4;

            // Enregistrez le classeur
            workbook.Save("ListColumnsDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListColumnCollection](../../listcolumncollection/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


