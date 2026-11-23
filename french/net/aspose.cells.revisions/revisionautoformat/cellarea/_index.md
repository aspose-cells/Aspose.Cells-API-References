---
title: "RevisionAutoFormat.CellArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionAutoFormat. Obtient l'emplacement où le formatage a été appliqué"
type: docs
url: /fr/net/aspose.cells.revisions/revisionautoformat/cellarea/
---
## RevisionAutoFormat.CellArea property

Obtient l'emplacement où le formatage a été appliqué.

```csharp
public CellArea CellArea { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionAutoFormatPropertyCellAreaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec suivi des révisions
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la collection des journaux de révision
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                
                // Trouvez la première instance de RevisionAutoFormat
                RevisionAutoFormat revisionFormat = null;
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionAutoFormat)
                        {
                            revisionFormat = (RevisionAutoFormat)revision;
                            break;
                        }
                    }
                    if (revisionFormat != null) break;
                }

                if (revisionFormat != null)
                {
                    // Démontrez la propriété CellArea (lecture seule)
                    CellArea area = revisionFormat.CellArea;
                    Console.WriteLine($"Formatting applied to area: StartRow={area.StartRow}, " +
                                      $"StartColumn={area.StartColumn}, EndRow={area.EndRow}, " +
                                      $"EndColumn={area.EndColumn}");
                }
                else
                {
                    Console.WriteLine("No auto-format revisions found in the workbook");
                }
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionAutoFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


