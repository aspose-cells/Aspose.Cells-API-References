---
title: "Style.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Style. Détermine si deux instances de Style sont égales"
type: docs
url: /fr/net/aspose.cells/style/equals/
---
## Style.Equals method

Détermine si deux instances de Style sont égales.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Object | L'objet Style à comparer avec l'objet Style actuel. |

### Valeur de retour

true si l'Objet spécifié est égal à l'Objet actuel ; sinon, false.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer deux styles à comparer
            Style style1 = workbook.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            style1.HorizontalAlignment = TextAlignmentType.Center;

            Style style2 = workbook.CreateStyle();
            style2.Font.Name = "Arial";
            style2.Font.Size = 12;
            style2.HorizontalAlignment = TextAlignmentType.Center;

            try
            {
                // Appeler la méthode Equals pour comparer les styles
                bool areEqual = style1.Equals((object)style2);

                // Afficher le résultat
                Console.WriteLine($"The styles are equal: {areEqual}");

                // Appliquer les styles pour démontrer qu'ils sont identiques
                if (areEqual)
                {
                    Cell cell1 = worksheet.Cells["A1"];
                    cell1.PutValue("Style 1");
                    cell1.SetStyle(style1);

                    Cell cell2 = worksheet.Cells["A2"];
                    cell2.PutValue("Style 2");
                    cell2.SetStyle(style2);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("StyleEqualsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


