---
title: "Classe RevisionFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Revisions.RevisionFormat classe. Représente un enregistrement de révision d'informations sur une modification de formatage"
type: docs
url: /fr/net/aspose.cells.revisions/revisionformat/
---
## RevisionFormat class

Représente un enregistrement de révision d'informations sur une modification de formatage.

```csharp
public class RevisionFormat : Revision
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Areas](../../aspose.cells.revisions/revisionformat/areas/) { get; } | La plage à laquelle ce formatage a été appliqué. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtient le numéro de cette révision.(Hérité de [`Revision`](../revision/).) |
| [Style](../../aspose.cells.revisions/revisionformat/style/) { get; } | Obtient le style appliqué. |
| override [Type](../../aspose.cells.revisions/revisionformat/type/) { get; } | Obtient le type de révision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtient la feuille de calcul. (Hérité de [`Revision`](../revision/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionFormatDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur en mode partagé pour activer le suivi des révisions
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajoutez des données et appliquez un formatage pour créer une révision
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("Sample Data");

                // Appliquez un style pour créer une révision de format
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                cell.SetStyle(style);

                // Accédez aux journaux de révision
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Affichez les propriétés de la révision
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);

                            // Afficher les informations de style
                            Style revisionStyle = revisionFormat.Style;
                            Console.WriteLine("Font Name: " + revisionStyle.Font.Name);
                            Console.WriteLine("Font Size: " + revisionStyle.Font.Size);
                            Console.WriteLine("Is Bold: " + revisionStyle.Font.IsBold);
                        }
                    }
                }

                // Enregistrez le classeur
                workbook.Save("RevisionFormatDemo.xlsx");
                Console.WriteLine("RevisionFormat demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionFormat: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


