---
title: "DocxSaveOptions.SaveElementType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DocxSaveOptions. Indique quels éléments doivent être enregistrés"
type: docs
url: /fr/net/aspose.cells/docxsaveoptions/saveelementtype/
---
## DocxSaveOptions.SaveElementType property

Indique quels éléments doivent être enregistrés.

```csharp
public SaveElementType SaveElementType { get; set; }
```

### Exemples

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveElementTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et ajouter des données d’exemple
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // Initialiser DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // NOTE : La propriété SaveElementType n’est pas présente dans la classe DocxSaveOptions
                // basé sur la réflexion d’API fournie. Si elle existait, vous la liriez ainsi :
                // var elementType = saveOptions.SaveElementType;
                // Console.WriteLine("SaveElementType: " + elementType);

                // Démontrer la lecture d’une propriété existante : SaveAsEditableShaps
                Console.WriteLine("SaveAsEditableShaps (default): " + saveOptions.SaveAsEditableShaps);

                // Définir la propriété sur true et afficher la nouvelle valeur
                saveOptions.SaveAsEditableShaps = true;
                Console.WriteLine("SaveAsEditableShaps (after set): " + saveOptions.SaveAsEditableShaps);

                // Enregistrer le classeur au format DOCX en utilisant les options configurées
                workbook.Save("SaveElementTypeDemo.docx", saveOptions);
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* enum [SaveElementType](../../../aspose.cells.saving/saveelementtype/)
* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


