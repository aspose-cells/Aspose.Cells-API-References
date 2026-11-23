---
title: "Classe OdsCellField"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Ods.OdsCellField. Représente le champ de cellule d'ods"
type: docs
url: /fr/net/aspose.cells.ods/odscellfield/
---
## OdsCellField class

Représente le champ de cellule d'ods.

```csharp
public class OdsCellField
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Column](../../aspose.cells.ods/odscellfield/column/) { get; set; } | Obtient et définit l'index de colonne de la cellule. |
| [CustomFormat](../../aspose.cells.ods/odscellfield/customformat/) { get; set; } | Représente le format personnalisé de la valeur du champ. |
| [FieldType](../../aspose.cells.ods/odscellfield/fieldtype/) { get; set; } | Obtient et définit le type du champ. |
| [Row](../../aspose.cells.ods/odscellfield/row/) { get; set; } | Obtient et définit l'index de ligne de la cellule. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Ods;

    public class OdsClassOdsCellFieldDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // -----------------------------------------------------------------
                // 1. Créez un OdsCellField via la collection (pas de constructeur sans paramètres)
                // -----------------------------------------------------------------
                OdsCellFieldCollection odsFields = sheet.Cells.OdsCellFields;
                odsFields.Add(2, 1, OdsCellFieldType.Title, "Demo Title");

                // Récupérez le champ que nous venons d'ajouter
                OdsCellField manualField = odsFields[odsFields.Count - 1];

                // Écrivez quelque chose dans la cellule identifiée par le OdsCellField
                sheet.Cells[manualField.Row, manualField.Column].PutValue("Manual Field");

                // --------------------------------------------------------------
                // 2. Ajoutez à nouveau le même champ pour démontrer l'utilisation de la collection (optionnel)
                // --------------------------------------------------------------
                odsFields.Add(manualField.Row, manualField.Column, manualField.FieldType, manualField.CustomFormat);

                // Mettez à jour tous les champs ODS afin qu'ils soient reflétés dans le fichier enregistré
                odsFields.UpdateFieldsValue();

                // Affichez les valeurs des propriétés dans la console
                Console.WriteLine($"Created OdsCellField -> Row: {manualField.Row}, Column: {manualField.Column}, " +
                                  $"Type: {manualField.FieldType}, Format: {manualField.CustomFormat}");

                // Enregistrez le classeur en tant que fichier ODS
                workbook.Save("OdsClassOdsCellFieldDemo.ods");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with OdsCellField: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


