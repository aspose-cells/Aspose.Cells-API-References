---
title: "ListObjectCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListObjectCollection. Obtient le ListObject par indice"
type: docs
url: /fr/net/aspose.cells.tables/listobjectcollection/item/
---
## ListObjectCollection indexer (1 of 2)

Obtient le ListObject par indice.

```csharp
public ListObject this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Valeur de retour

Le ListObject

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Créer un objet de liste
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Accéder à l'objet de liste en utilisant la propriété Item
            ListObject firstListObject = worksheet.ListObjects[0];
            
            // Définir le style du tableau
            firstListObject.TableStyleType = TableStyleType.TableStyleMedium2;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ListObjectCollection indexer (2 of 2)

Obtient le ListObject par le nom spécifié.

```csharp
public ListObject this[string tableName] { get; }
```

| Paramètre | Description |
| --- | --- |
| tableName | Nom du ListObject. |

### Valeur de retour

Le ListObject

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Créer un objet de liste
            int index = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject listObj = worksheet.ListObjects[index];
            listObj.DisplayName = "PersonTable";

            // Accéder à l'objet de liste en utilisant la propriété Item par nom
            ListObject retrievedListObj = worksheet.ListObjects["PersonTable"];
            
            // Démontrer l'utilisation en convertissant en plage
            retrievedListObj.ConvertToRange();

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


