---
title: "Cells.DeleteBlankRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Supprime toutes les lignes vides qui ne contiennent aucune donnée ni aucun autre objet"
type: docs
url: /fr/net/aspose.cells/cells/deleteblankrows/
---
## DeleteBlankRows() {#deleteblankrows}

Supprime toutes les lignes vides qui ne contiennent aucune donnée ou autre objet.

```csharp
public void DeleteBlankRows()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajoutez des données avec des lignes vides
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A4"].PutValue("Data2"); // Blank row at A3
            cells["A6"].PutValue("Data3"); // Blank row at A5

            Console.WriteLine("Before deleting blank rows:");
            for (int i = 0; i < 7; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

            // Supprimez les lignes vides
            cells.DeleteBlankRows();

            Console.WriteLine("\nAfter deleting blank rows:");
            for (int i = 0; i < cells.MaxDataRow + 1; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteBlankRows(DeleteOptions) {#deleteblankrows_1}

Supprime toutes les lignes vides qui ne contiennent aucune donnée ou certains objets spéciaux tels que les commentaires visibles, les tableaux croisés dynamiques.

```csharp
public void DeleteBlankRows(DeleteOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | DeleteOptions | Les options de suppression de la plage. |

### Remarques

Pour les lignes vides qui seront supprimées, il ne suffit pas que [`IsBlank`](../../row/isblank/) soit vrai, il faut également qu’aucun commentaire visible ne soit défini pour aucune cellule de ces lignes, et qu’aucun tableau croisé dynamique dont la plage intersecte celles‑ci ne soit présent.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsWithDeleteOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajoutez des données de test avec des lignes vides
            sheet.Cells["A1"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A5"].PutValue("Data3");
            
            // Créez des options de suppression
            DeleteOptions options = new DeleteOptions();
            options.UpdateReference = true;
            
            // Supprimez les lignes vides
            sheet.Cells.DeleteBlankRows(options);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


