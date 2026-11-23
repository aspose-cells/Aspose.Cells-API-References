---
title: "StyleFlag.HideFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Le paramètre Hide formula sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/hideformula/
---
## StyleFlag.HideFormula property

Le paramètre de masquage de formule sera appliqué.

```csharp
public bool HideFormula { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyHideFormulaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell a1 = worksheet.Cells["A1"];
            // Ajouter une formule à la cellule A1
            a1.Formula = "=1+2";
            a1.Value = 3; // Display value

            // Créer un style flag avec HideFormula défini sur true
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HideFormula = true;

            // Créer un style et définir IsFormulaHidden sur true
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;

            // Appliquer le style à la cellule A1 avec le style flag
            a1.SetStyle(style, styleFlag);

            // Protéger la feuille de calcul pour voir l'effet de HideFormula
            worksheet.Protection.AllowEditingObject = true;
            worksheet.Protection.AllowEditingContent = false;
            worksheet.Protection.Password = "password";

            // Enregistrez le classeur
            workbook.Save("PropertyHideFormulaDemo.xlsx");

            // Vérifier que la formule est masquée
            Console.WriteLine("Formula in A1: " + a1.Formula);
            Console.WriteLine("Is formula hidden? " + a1.GetStyle().IsFormulaHidden);
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


