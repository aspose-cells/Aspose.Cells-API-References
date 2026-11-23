---
title: "DocxSaveOptions.SaveAsEditableShapes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DocxSaveOptions. Enregistrer tous les objets de dessin en tant que formes éditables dans le fichier Word afin que vous puissiez les modifier dans Word"
type: docs
url: /fr/net/aspose.cells/docxsaveoptions/saveaseditableshapes/
---
## DocxSaveOptions.SaveAsEditableShapes property

Enregistrez tous les objets de dessin comme formes modifiables dans le fichier Word, afin de pouvoir les modifier dans Word.

```csharp
public bool SaveAsEditableShapes { get; set; }
```

### Remarques

Uniquement pour les graphiques.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertySaveAsEditableShapesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul et ajouter des données d’exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Editable Shapes Demo";

            try
            {
                // Initialiser DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Afficher la valeur par défaut de la propriété SaveAsEditableShapes
                Console.WriteLine("Default SaveAsEditableShapes value: " + saveOptions.SaveAsEditableShapes);

                // Définir SaveAsEditableShapes sur true pour démontrer son utilisation
                saveOptions.SaveAsEditableShapes = true;
                Console.WriteLine("SaveAsEditableShapes set to: " + saveOptions.SaveAsEditableShapes);

                // Enregistrer le classeur au format DOCX avec les options configurées
                workbook.Save("SaveAsEditableShapesDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with SaveAsEditableShapes option.");
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

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


