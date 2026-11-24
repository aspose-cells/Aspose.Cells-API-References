---
title: "RevisionDefinedName.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionDefinedName-Eigenschaft. Stellt den Typ der Revision dar"
type: docs
url: /de/net/aspose.cells.revisions/revisiondefinedname/type/
---
## RevisionDefinedName.Type property

Stellt den Typ der Revision dar.

```csharp
public override RevisionType Type { get; }
```

### Beispiele

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
                // Erstellen Sie eine neue Arbeitsmappe und fügen Sie einen definierten Namen hinzu
                Workbook wb = new Workbook();
                Worksheet ws = wb.Worksheets[0];

                int nameIdx = wb.Worksheets.Names.Add("DemoName");
                Name definedName = wb.Worksheets.Names[nameIdx];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Ändern Sie den definierten Namen, um einen Revisionsdatensatz zu erzeugen
                definedName.RefersTo = "=Sheet1!$B$1";

                // Speichern Sie die Arbeitsmappe, um Revisionsinformationen einzubetten
                string filePath = "RevisionDefinedName_TypeDemo.xlsx";
                wb.Save(filePath);

                // Öffnen Sie die Arbeitsmappe erneut, um das Revisionsprotokoll zu lesen
                Workbook revWb = new Workbook(filePath);

                // Durchlaufen Sie die Revisionen und zeigen Sie den Type jedes RevisionDefinedName‑Eintrags an
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

### Siehe auch

* enum [RevisionType](../../revisiontype/)
* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


