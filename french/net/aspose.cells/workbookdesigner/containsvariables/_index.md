---
title: "WorkbookDesigner.ContainsVariables"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookDesigner. Indique si la première feuille de calcul contient des variables personnalisées"
type: docs
url: /fr/net/aspose.cells/workbookdesigner/containsvariables/
---
## WorkbookDesigner.ContainsVariables property

Indique si la première feuille de calcul contient des variables personnalisées.

```csharp
[Obsolete("Use WorkbookDesigner.VariablesWorksheetName property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ContainsVariables { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété WorkbookDesigner.VariablesWorksheetName. Cette propriété sera supprimée trois mois plus tard, à compter de septembre 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyContainsVariablesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une feuille de calcul d’exemple
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour rendre l’exemple significatif
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Créer une instance de WorkbookDesigner
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Afficher la valeur actuelle de la propriété ContainsVariables
                Console.WriteLine("Initial ContainsVariables value: " + designer.ContainsVariables);

                // Définir la propriété ContainsVariables sur true
                designer.ContainsVariables = true;

                // Afficher la valeur mise à jour
                Console.WriteLine("Updated ContainsVariables value: " + designer.ContainsVariables);

                // Enregistrer le résultat
                workbook.Save("ContainsVariablesDemo.xlsx");

                Console.WriteLine("ContainsVariables property has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


