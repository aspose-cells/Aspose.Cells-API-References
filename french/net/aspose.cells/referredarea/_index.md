---
title: "Classe ReferredArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ReferredArea class. Représente une zone référencée par la formule"
type: docs
url: /fr/net/aspose.cells/referredarea/
---
## ReferredArea class

Représente une zone référencée par la formule.

```csharp
public class ReferredArea
```

## Propriétés

| Nom | Description |
| --- | --- |
| [EndColumn](../../aspose.cells/referredarea/endcolumn/) { get; } | La colonne de fin de la zone. |
| [EndRow](../../aspose.cells/referredarea/endrow/) { get; } | La ligne de fin de la zone. |
| [ExternalFileName](../../aspose.cells/referredarea/externalfilename/) { get; } | Obtenir le nom du fichier externe si c'est une référence externe. |
| [IsArea](../../aspose.cells/referredarea/isarea/) { get; } | Indique si c'est une zone. |
| [IsEntireColumn](../../aspose.cells/referredarea/isentirecolumn/) { get; } | Indique si cette zone contient toutes les lignes (colonne entière). |
| [IsEntireRow](../../aspose.cells/referredarea/isentirerow/) { get; } | Indique si cette zone contient toutes les colonnes (ligne entière). |
| [IsExternalLink](../../aspose.cells/referredarea/isexternallink/) { get; } | Indique si c'est un lien externe. |
| [SheetName](../../aspose.cells/referredarea/sheetname/) { get; } | Indique dans quelle feuille se trouve cette référence. |
| [SheetNames](../../aspose.cells/referredarea/sheetnames/) { get; } | Noms de toutes les feuilles de calcul auxquelles cette instance fait référence. |
| [StartColumn](../../aspose.cells/referredarea/startcolumn/) { get; } | La colonne de départ de la zone. |
| [StartRow](../../aspose.cells/referredarea/startrow/) { get; } | La ligne de départ de la zone. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue)(int, int) | Obtient la valeur de la cellule avec le décalage donné depuis le coin supérieur gauche de cette zone. |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue_1)(int, int, bool) | Obtient la valeur de la cellule avec le décalage donné depuis le coin supérieur gauche de cette zone. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues)() | Obtient les valeurs des cellules dans cette zone. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues_1)(bool) | Obtient les valeurs des cellules dans cette zone. |
| override [ToString](../../aspose.cells/referredarea/tostring/)() | Renvoie l'adresse de référence de cette zone. En général, il s'agit de l'adresse de la référence qui peut être utilisée dans une formule, comme "Sheet1!A1:C3". |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassReferredAreaDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Configurez des données et une formule qui fait référence à une plage
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["B1"].PutValue(30);
                worksheet.Cells["B2"].PutValue(40);

                // Créez une formule qui fait référence à la plage A1:B2
                Cell formulaCell = worksheet.Cells["C1"];
                formulaCell.Formula = "=SUM(A1:B2)";

                // Obtenez les zones référencées à partir de la formule
                ReferredAreaCollection referredAreas = formulaCell.GetPrecedents();
                if (referredAreas.Count > 0)
                {
                    // Obtenez la première zone référencée
                    ReferredArea referredArea = referredAreas[0];

                    // Affichez les propriétés de base de la zone référencée
                    Console.WriteLine($"Referred Area Details:");
                    Console.WriteLine($"- Is External Link: {referredArea.IsExternalLink}");
                    Console.WriteLine($"- Sheet Name: {referredArea.SheetName}");
                    Console.WriteLine($"- Start Row: {referredArea.StartRow}");
                    Console.WriteLine($"- Start Column: {referredArea.StartColumn}");
                    Console.WriteLine($"- End Row: {referredArea.EndRow}");
                    Console.WriteLine($"- End Column: {referredArea.EndColumn}");
                    Console.WriteLine($"- Is Area: {referredArea.IsArea}");
                    Console.WriteLine($"- Is Entire Row: {referredArea.IsEntireRow}");
                    Console.WriteLine($"- Is Entire Column: {referredArea.IsEntireColumn}");

                    // Obtenez les valeurs de la zone référencée
                    object values = referredArea.GetValues();
                    if (values is Array)
                    {
                        object[][] valueArray = (object[][])values;
                        Console.WriteLine("\nValues in the referred area:");
                        foreach (object[] row in valueArray)
                        {
                            foreach (object val in row)
                            {
                                Console.Write($"{val}\t");
                            }
                            Console.WriteLine();
                        }
                    }

                    // Obtenez une valeur spécifique de la zone référencée
                    object specificValue = referredArea.GetValue(0, 1);
                    Console.WriteLine($"\nValue at row 0, column 1: {specificValue}");

                    // Affichez l'adresse de référence
                    Console.WriteLine($"Reference address: {referredArea.ToString()}");
                }

                // Enregistrez le classeur
                workbook.Save("ReferredAreaDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ReferredArea: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


