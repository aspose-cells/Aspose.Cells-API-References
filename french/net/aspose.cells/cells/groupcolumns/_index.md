---
title: "Cells.GroupColumns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Regroupe les colonnes"
type: docs
url: /fr/net/aspose.cells/cells/groupcolumns/
---
## GroupColumns(int, int) {#groupcolumns}

Regroupe les colonnes.

```csharp
public void GroupColumns(int firstIndex, int lastIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | Le premier indice de colonne à regrouper. |
| lastIndex | Int32 | Le dernier indice de colonne à regrouper. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Regrouper les colonnes de l'indice 0 à 255
            cells.GroupColumns(0, 255);

            // Enregistrez le classeur
            string outputPath = "outputGroupColumns.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Columns grouped successfully. File saved to: " + outputPath);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupColumns(int, int, bool) {#groupcolumns_1}

Regroupe les colonnes.

```csharp
public void GroupColumns(int firstIndex, int lastIndex, bool isHidden)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | Le premier indice de colonne à regrouper. |
| lastIndex | Int32 | Le dernier indice de colonne à regrouper. |
| isHidden | Boolean | Spécifie si les colonnes regroupées sont masquées. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Regrouper les colonnes 5 à 7 (3 colonnes) et les masquer
            cells.GroupColumns(5, 7, true);

            // Enregistrez le classeur
            workbook.Save("GroupColumnsOutput.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


