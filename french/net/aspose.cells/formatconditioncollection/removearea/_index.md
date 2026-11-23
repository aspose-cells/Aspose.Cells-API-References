---
title: "FormatConditionCollection.RemoveArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FormatConditionCollection. Supprime la plage de cellules formatées conditionnellement par indice"
type: docs
url: /fr/net/aspose.cells/formatconditioncollection/removearea/
---
## RemoveArea(int) {#removearea_1}

Supprime la plage de cellules formatée conditionnellement par index.

```csharp
public void RemoveArea(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'indice de la plage de cellules formatées conditionnellement à supprimer. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une mise en forme conditionnelle
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];

            // Ajouter des zones à formater
            formatConditionCollection.AddArea(CellArea.CreateCellArea(0, 0, 10, 5)); // First area
            formatConditionCollection.AddArea(CellArea.CreateCellArea(5, 5, 15, 10)); // Second area

            // Ajouter une condition
            formatConditionCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");

            // Afficher le nombre de zones initial (nous savons que nous avons ajouté 2 zones)
            Console.WriteLine("Areas before removal: 2");

            // Supprimer la deuxième zone (indice 1)
            formatConditionCollection.RemoveArea(1);

            // Afficher le nombre de zones après suppression (nous savons que nous avons supprimé 1 zone)
            Console.WriteLine("Areas after removal: 1");

            // Enregistrez le classeur
            workbook.Save("RemoveAreaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveArea(int, int, int, int) {#removearea}

Supprimer le formatage conditionnel dans la plage.

```csharp
public bool RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | La startRow de la plage. |
| startColumn | Int32 | La startColumn de la plage. |
| totalRows | Int32 | Le nombre de lignes de la plage. |
| totalColumns | Int32 | Le nombre de colonnes de la plage. |

### Valeur de retour

Renvoie TRUE, cette FormatCondtionCollection doit être supprimée.

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            
            int idx = cfc.Add();
            FormatConditionCollection fcc = cfc[idx];
            
            // Ajouter la zone initiale
            CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
            fcc.AddArea(initialArea);
            
            // Ajouter une condition
            idx = fcc.AddCondition(FormatConditionType.Expression);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "=A1>0";
            fc.Style.Font.Color = Color.Red;
            
            // Démontrer RemoveArea avec des paramètres Int32
            Console.WriteLine("Before removal - Areas count: " + fcc.Count);
            fcc.RemoveArea(0, 0, 1, 1); // Remove the initial area
            Console.WriteLine("After removal - Areas count: " + fcc.Count);
            
            // Ajouter une nouvelle zone
            CellArea newArea = CellArea.CreateCellArea(1, 1, 1, 1);
            fcc.AddArea(newArea);
            Console.WriteLine("After adding new area - Areas count: " + fcc.Count);
        }
    }
}
```

### Voir aussi

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


