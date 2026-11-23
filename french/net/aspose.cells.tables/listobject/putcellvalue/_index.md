---
title: "ListObject.PutCellValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ListObject. Mettre la valeur dans la cellule"
type: docs
url: /fr/net/aspose.cells.tables/listobject/putcellvalue/
---
## PutCellValue(int, int, object) {#putcellvalue}

Placez la valeur dans la cellule.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | Le décalage de ligne dans le tableau. |
| columnOffset | Int32 | Le décalage de colonne dans le tableau. |
| valeur | Object | La valeur de la cellule. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellValueWithInt32Int32ObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["C2"].PutValue(300);

            // Créer un objet de liste
            int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Démontrer PutCellValue avec les paramètres Int32, Int32, Object
            listObject.PutCellValue(1, 0, 500); // Update row 1, column 0 with value 500
            listObject.PutCellValue(1, 1, "Updated Value"); // Update row 1, column 1 with string
            listObject.PutCellValue(1, 2, DateTime.Now); // Update row 1, column 2 with current date

            // Enregistrez le classeur
            workbook.Save("ListObjectPutCellValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellValue(int, int, object, bool) {#putcellvalue_1}

Placez la valeur dans la cellule.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value, bool isTotalsRowLabel)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | Le décalage de ligne dans le tableau. |
| columnOffset | Int32 | Le décalage de colonne dans le tableau. |
| valeur | Object | La valeur de la cellule. |
| isTotalsRowLabel | Boolean | Indique s'il s'agit d'une étiquette pour la ligne totale, ne fonctionne que pour la ligne totale. Si False et que cette ligne est une ligne totale, une nouvelle ligne sera insérée. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellValueWithInt32Int32ObjectBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour créer un ListObject
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");
            
            // Créer un ListObject
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Utiliser PutCellValue pour mettre à jour une cellule (ligne 2, colonne 1) avec une nouvelle valeur et étendre le tableau
            listObject.PutCellValue(2, 1, "Updated Value", true);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


