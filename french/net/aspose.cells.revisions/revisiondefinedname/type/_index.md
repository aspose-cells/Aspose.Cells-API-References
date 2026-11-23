---
title: "RevisionDefinedName.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionDefinedName. Représente le type de révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisiondefinedname/type/
---
## RevisionDefinedName.Type property

Représente le type de révision.

```csharp
public override RevisionType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionDefinedNamePropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Créez un nouveau classeur et ajoutez un nom défini
                Workbook wb = new Workbook();
                Worksheet ws = wb.Worksheets[0];

                int nameIdx = wb.Worksheets.Names.Add("DemoName");
                Name definedName = wb.Worksheets.Names[nameIdx];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Modifiez le nom défini pour générer un enregistrement de révision
                definedName.RefersTo = "=Sheet1!$B$1";

                // Enregistrez le classeur pour intégrer les informations de révision
                string filePath = "RevisionDefinedName_TypeDemo.xlsx";
                wb.Save(filePath);

                // Rouvrez le classeur pour lire le journal de révision
                Workbook revWb = new Workbook(filePath);

                // Itérez à travers les révisions et affichez le Type de chaque entrée RevisionDefinedName
                foreach (RevisionLog log in revWb.Worksheets.RevisionLogs)
                {
                    foreach (Revision rev in log.Revisions)
                    {
                        if (rev.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName rdn = (RevisionDefinedName)rev;
                            Console.WriteLine($"Revision Type: {rdn.Type}");
                            Console.WriteLine($"Defined Name Text: {rdn.Text}");
                            Console.WriteLine($"Old Formula: {rdn.OldFormula}");
                            Console.WriteLine($"New Formula: {rdn.NewFormula}");
                        }
                    }
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


