---
title: "WorksheetCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorksheetCollection. Obtient l'élément Worksheet à l'index spécifié"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/item/
---
## WorksheetCollection indexer (1 of 2)

Obtient l'élément [`Worksheet`](../../worksheet/) à l'index spécifié.

```csharp
public Worksheet this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Utilisation de la propriété Item pour accéder à la cellule
            Cell cell = cells[0, 0];
            cell.Formula = "=SUM(1, 2, 3)";
            
            workbook.CalculateFormula();
            Console.WriteLine("Cell value: " + cell.IntValue);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorksheetCollection indexer (2 of 2)

Obtient l'élément [`Worksheet`](../../worksheet/) avec le nom spécifié.

```csharp
public Worksheet this[string sheetName] { get; }
```

| Paramètre | Description |
| --- | --- |
| sheetName | Nom de la feuille de calcul |

### Valeur de retour

L'élément avec le nom spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder aux feuilles de calcul en utilisant la propriété Item par index et par nom
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            
            // Accéder à la feuille de calcul par nom en utilisant la propriété Item
            Worksheet accessedSheet = workbook.Worksheets["FirstSheet"];
            
            // Ajouter des données pour démontrer l'accès aux feuilles de calcul
            Cells cells = accessedSheet.Cells;
            cells["A1"].PutValue("Worksheet accessed successfully!");
            cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Insérer une colonne dans la deuxième feuille
            workbook.Worksheets["SecondSheet"].Cells.InsertColumn(1);
            
            // Enregistrez le classeur
            workbook.Save("WorksheetCollectionItemDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


