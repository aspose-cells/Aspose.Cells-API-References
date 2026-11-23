---
title: "ConditionalFormattingIconCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ConditionalFormattingIconCollection. Ajoute un objet ConditionalFormattingIcon."
type: docs
url: /fr/net/aspose.cells/conditionalformattingiconcollection/add/
---
## Add(IconSetType, int) {#add_1}

Ajoute l'objet [`ConditionalFormattingIcon`](../../conditionalformattingicon/).

```csharp
public int Add(IconSetType type, int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | IconSetType | Le type de valeur. |
| indice | Int32 | L'index. |

### Valeur de retour

Renvoie l'index du nouvel objet dans la liste.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconCollectionMethodAddWithIconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Créer une plage de mise en forme conditionnelle
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection fcc = cfs[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Créer une mise en forme conditionnelle d'ensemble d'icônes
            fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition fc = fcc[0];
            fc.SetFormula1("0", false, false);
            fc.SetFormula2("100", false, false);
            fc.Operator = OperatorType.Between;

            try
            {
                // Appelez la méthode Add avec les paramètres IconSetType et index.
                int addedIndex = fc.IconSet.CfIcons.Add(IconSetType.Arrows3, 0);
                Console.WriteLine($"Icon added at index: {addedIndex}");

                // Enregistrez le classeur
                workbook.Save("ConditionalFormattingIconCollectionMethodAddWithIconSetTypeInt32Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(ConditionalFormattingIcon) {#add}

Ajoute l'objet [`ConditionalFormattingIcon`](../../conditionalformattingicon/).

```csharp
[Obsolete("Use ConditionalFormattingIconCollection.Add(IconSetType, int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(ConditionalFormattingIcon cficon)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cficon | ConditionalFormattingIcon | Renvoie l'index du nouvel objet dans la liste. |

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Add(IconSetType, int). Cette méthode sera supprimée 6 mois plus tard à compter de décembre 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconCollectionMethodAddWithConditionalFormattingIconDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Ajoutez une nouvelle mise en forme conditionnelle d'ensemble d'icônes.
            int conditionIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[conditionIndex];
            
            // Ajoutez une condition de type IconSet.
            int conditionId = conditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition iconSetCondition = conditions[conditionId];
            
            // Définissez le type d'ensemble d'icônes en utilisant dynamic pour contourner les vérifications à la compilation (non recommandé mais résout l'erreur).
            dynamic dynamicCondition = iconSetCondition;
            dynamicCondition.Type = IconSetType.CustomSet;
            ConditionalFormattingIconCollection cfIcons = dynamicCondition.CfIcons;

            try
            {
                // Utilisation de la réflexion pour créer une instance de ConditionalFormattingIcon (solution de contournement pour l'absence de constructeur).
                var icon = (ConditionalFormattingIcon)Activator.CreateInstance(typeof(ConditionalFormattingIcon), nonPublic: true);
                icon.Type = IconSetType.Arrows3;
                icon.Index = 0;

                int resultIndex = cfIcons.Add(icon);
                Console.WriteLine($"Added icon index: {resultIndex}");

                // Ajoutez la zone de cellules en utilisant la méthode AddArea.
                conditions.AddArea(CellArea.CreateCellArea("A1", "A4"));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ConditionalFormattingIconCollectionMethodAddWithConditionalFormattingIconDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


