---
title: "ExportTableOptions.PreprocessExportedValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ExportTableOptions method. Prétraiter la valeur de la cellule actuelle à exporter"
type: docs
url: /fr/net/aspose.cells/exporttableoptions/preprocessexportedvalue/
---
## ExportTableOptions.PreprocessExportedValue method

Prétraitez la valeur de la cellule actuelle à exporter.

```csharp
public virtual bool PreprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellRow | Int32 | l'index de ligne de la cellule actuelle |
| cellColumn | Int32 | l'index de colonne de la cellule |
| valeur | CellValue | valeur et type de la cellule actuelle |

### Valeur de retour

Indique si la cellule actuelle a été remplacée par un type différent et/ou une valeur.

### Remarques

L'index de ligne et de colonne est l'index absolu de la cellule dans la feuille de calcul, pas l'index dans le tableau exporté. L'utilisateur peut vérifier la valeur de la cellule actuelle dans l'implémentation de substitution de cette méthode ; si la cellule actuelle doit être remplacée par un autre type et une autre valeur, l'implémentation doit alors définir le type et la valeur attendus dans l'objet CellValue et retourner true. Par défaut, cette méthode ne fait rien et retourne false.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExportTableOptionsMethodPreprocessExportedValueWithInt32Int32CellValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple dans la feuille de calcul
            worksheet.Cells["A1"].PutValue("Test Value");
            worksheet.Cells["A2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            // Créez une instance de ExportTableOptions
            ExportTableOptions exportOptions = new ExportTableOptions();

            // Créer un objet CellValue à des fins de démonstration
            CellValue cellValue = new CellValue();
            cellValue.Type = CellValueType.IsString;
            cellValue.Value = "Processed Value";

            try
            {
                // Appeler PreprocessExportedValue avec des paramètres spécifiques (ligne 0, colonne 0, CellValue)
                bool result = exportOptions.PreprocessExportedValue(0, 0, cellValue);

                // Afficher le résultat de l'appel de la méthode
                Console.WriteLine($"PreprocessExportedValue returned: {result}");

                // Modifier la cellule avec la valeur traitée si nécessaire
                if (result)
                {
                    worksheet.Cells[0, 0].PutValue(cellValue.Value);
                }

                // Enregistrez le classeur
                workbook.Save("PreprocessExportedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PreprocessExportedValue method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CellValue](../../cellvalue/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


