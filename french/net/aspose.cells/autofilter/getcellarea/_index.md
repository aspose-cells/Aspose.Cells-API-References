---
title: "AutoFilter.GetCellArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AutoFilter. Obtient la CellArea où cet AutoFilter s'applique"
type: docs
url: /fr/net/aspose.cells/autofilter/getcellarea/
---
## GetCellArea() {#getcellarea}

Obtient le [`CellArea`](../../cellarea/) où ce AutoFilter s'applique.

```csharp
public CellArea GetCellArea()
```

### Valeur de retour

la zone à laquelle ce filtre s'applique

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Remplir des données d'exemple pour la démonstration de l'AutoFilter
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Category");
            cells["C1"].PutValue("Price");

            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue("Fruit");
            cells["C2"].PutValue(2.5);

            cells["A3"].PutValue("Carrot");
            cells["B3"].PutValue("Vegetable");
            cells["C3"].PutValue(1.2);

            cells["A4"].PutValue("Banana");
            cells["B4"].PutValue("Fruit");
            cells["C4"].PutValue(3.1);

            // Appliquer l'AutoFilter aux en-têtes (indice de ligne 0) couvrant les colonnes A-C (0-2)
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.SetRange(0, 0, 2);

            try
            {
                // Obtenir le CellArea où l'AutoFilter est appliqué
                CellArea result = autoFilter.GetCellArea();

                // Afficher les coordonnées de la plage de l'AutoFilter
                Console.WriteLine("AutoFilter applied to cell area:");
                Console.WriteLine($"Start Row: {result.StartRow}");
                Console.WriteLine($"Start Column: {result.StartColumn}");
                Console.WriteLine($"End Row: {result.EndRow}");
                Console.WriteLine($"End Column: {result.EndColumn}");

                // Appliquer un filtre simple pour démontrer la fonctionnalité (optionnel)
                autoFilter.Filter(1, "Fruit"); // Filter "Category" column (index 1) for "Fruit"
                autoFilter.Refresh();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea method: {ex.Message}");
            }

            // Enregistrer le classeur avec l'AutoFilter appliqué
            workbook.Save("AutoFilterMethodGetCellAreaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellArea(bool) {#getcellarea_1}

Obtient le [`CellArea`](../../cellarea/) où l'AutoFilter spécifié s'applique.

```csharp
public CellArea GetCellArea(bool refreshAppliedRange)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| refreshAppliedRange | Boolean | Indique s'il faut rafraîchir la plage appliquée. Pour la plage appliquée du AutoFilter, la dernière ligne peut changer lorsque les données des cellules changent. Si ce drapeau est vrai, alors la dernière ligne de la plage sera recalculée en fonction des données actuelles des cellules. |

### Valeur de retour

la zone à laquelle ce filtre s'applique

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparer des données d'exemple pour l'AutoFilter
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");

            // Définir la plage de l'AutoFilter (ligne 0 à 3, colonne 0)
            worksheet.AutoFilter.SetRange(0, 0, 0);

            try
            {
                // Appeler GetCellArea avec refreshAppliedRange=true
                CellArea result = worksheet.AutoFilter.GetCellArea(true);

                // Afficher la plage appliquée de l'AutoFilter
                Console.WriteLine($"AutoFilter Range: StartRow={result.StartRow}, " +
                    $"StartColumn={result.StartColumn}, EndRow={result.EndRow}, " +
                    $"EndColumn={result.EndColumn}");

                Console.WriteLine("GetCellArea method executed successfully with boolean parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("AutoFilterMethodGetCellAreaWithBooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


