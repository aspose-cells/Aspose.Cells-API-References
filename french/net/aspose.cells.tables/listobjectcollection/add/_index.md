---
title: "ListObjectCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ListObjectCollection. Ajoute un ListObject à la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.tables/listobjectcollection/add/
---
## Add(int, int, int, int, bool) {#add}

Ajoute un ListObject à la feuille de calcul.

```csharp
public int Add(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | La ligne de départ de la plage de liste. |
| startColumn | Int32 | La ligne de départ de la plage de liste. |
| endRow | Int32 | La ligne de départ de la plage de liste. |
| endColumn | Int32 | La ligne de départ de la plage de liste. |
| hasHeaders | Boolean | Indique si la plage possède des en-têtes. |

### Valeur de retour

L'index du nouveau ListObject

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir des données dans une plage
            var range = worksheet.Cells.CreateRange("B3:D4");
            range.Value = new object[,]
            {
                {"Col1", "Col2", "Col3"},
                {100, 200, 300}
            };

            // Ajouter ListObject en utilisant la méthode Add avec des paramètres Int32
            int firstRow = range.FirstRow;
            int firstColumn = range.FirstColumn;
            int endRow = firstRow + range.RowCount - 1;
            int endColumn = firstColumn + range.ColumnCount - 1;
            worksheet.ListObjects.Add(firstRow, firstColumn, endRow, endColumn, true);

            // Activer les totaux et définir la formule pour une colonne
            worksheet.ListObjects[0].ShowTotals = true;
            worksheet.Cells["D5"].Formula = "=SUBTOTAL(109,[Col3])";

            // Enregistrez le classeur
            workbook.Save("ListObjectAddDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, bool) {#add_1}

Ajoute un ListObject à la feuille de calcul.

```csharp
public int Add(string startCell, string endCell, bool hasHeaders)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startCell | String | La cellule de départ de la plage de la liste. |
| endCell | String | La cellule de fin de la plage de la liste. |
| hasHeaders | Boolean | Indique si la plage possède des en-têtes. |

### Valeur de retour

L'index du nouveau ListObject

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithStringStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplissez des données d'exemple
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);

            // Ajouter l'objet de liste en utilisant des références de plage de chaîne
            ListObjectCollection listObjects = worksheet.ListObjects;
            listObjects.Add("A1", "B3", true);
            
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


