---
title: "Validation.AddArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Validation. Applique la validation à la zone"
type: docs
url: /fr/net/aspose.cells/validation/addarea/
---
## AddArea(CellArea) {#addarea}

Applique la validation à la zone.

```csharp
public void AddArea(CellArea cellArea)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | La zone. |

### Remarques

C’est équivalent d’utiliser `AddArea` avec la vérification de l’intersection et du bord.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Créer une validation
            ValidationCollection vc = sheet.Validations;
            Validation validation = vc[vc.Add(CellArea.CreateCellArea(0, 0, 0, 0))];
            validation.Type = ValidationType.List;
            validation.Formula1 = "=A1:A10";

            // Ajouter plus de zones à la validation
            for (int i = 1; i < 5; i++)
            {
                validation.AddArea(CellArea.CreateCellArea(i, 0, i, 0));
            }

            // Enregistrez le classeur
            wb.Save("ValidationMethodAddAreaWithCellAreaDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Validation with multiple areas created successfully.");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddArea(CellArea, bool, bool) {#addarea_1}

Applique la validation à la zone.

```csharp
public void AddArea(CellArea cellArea, bool checkIntersection, bool checkEdge)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | La zone. |
| checkIntersection | Boolean | Indique s'il faut vérifier l'intersection de la zone donnée avec les zones des validations existantes. Si une validation a été appliquée dans la zone donnée (ou une partie de celle‑ci), alors la validation existante doit d'abord être supprimée de la zone donnée. Sinon, une corruption peut être causée pour les validations générées. Si l'utilisateur est sûr que la zone ajoutée n'intersecte aucune zone existante, ce paramètre peut être défini sur false pour des considérations de performance. |
| checkEdge | Boolean | Indique s'il faut vérifier le bord des zones appliquées de cette validation. Les paramètres internes de Validation dépendent de la zone en haut à gauche de ses plages appliquées, ainsi si la zone donnée devient la nouvelle zone en haut à gauche des plages appliquées, les paramètres internes doivent être modifiés et reconstruits, sinon un résultat inattendu peut survenir. Si l'utilisateur est sûr que la zone ajoutée n'est pas la zone en haut à gauche, ce paramètre peut être défini sur false pour des considérations de performance. |

### Remarques

Dans cette méthode, nous supprimerons toutes les anciennes validations dans la zone donnée. Pour la zone en haut à gauche des plages appliquées de Validation, d'abord son StartRow est le plus petit, ensuite son StartColumn est le plus petit parmi les zones qui ont le même StartRow minimal.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur et obtenir la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une validation dans une zone spécifique
            Validation validation = worksheet.Validations[worksheet.Validations.Add(CellArea.CreateCellArea(5, 3, 6, 3))];
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "F3";

            // Démontrer AddArea avec CellArea et deux paramètres booléens
            validation.AddArea(CellArea.CreateCellArea(3, 3, 3, 4), false, true);
            Console.WriteLine("Area count after AddArea: " + validation.Areas.Length);
            Console.WriteLine("Formula1 after AddArea: " + validation.Formula1);

            // Supprimer la zone ajoutée
            validation.RemoveArea(CellArea.CreateCellArea(3, 3, 3, 4));
            Console.WriteLine("Area count after RemoveArea: " + validation.Areas.Length);

            // Ajouter plusieurs zones avec une opération en masse
            CellArea[] areas = new CellArea[10];
            for (int i = 0; i < areas.Length; i++)
            {
                areas[i] = CellArea.CreateCellArea(6 + i, 3, 6 + i, 4);
            }
            validation.AddAreas(areas, true, true);
            Console.WriteLine("Area count after bulk AddAreas: " + validation.Areas.Length);

            // Enregistrez le classeur
            workbook.Save("ValidationMethodAddAreaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


