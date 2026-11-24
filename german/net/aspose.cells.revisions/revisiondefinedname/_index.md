---
title: "Klasse RevisionDefinedName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.RevisionDefinedName Klasse. Stellt einen Revisionsdatensatz einer definierten Namensänderung dar"
type: docs
url: /de/net/aspose.cells.revisions/revisiondefinedname/
---
## RevisionDefinedName class

Stellt einen Revisionsdatensatz einer definierten Namensänderung dar.

```csharp
public class RevisionDefinedName : Revision
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ermittelt die Nummer dieser Revision.(Vererbt von [`Revision`](../revision/).) |
| [NewFormula](../../aspose.cells.revisions/revisiondefinedname/newformula/) { get; } | Liest die Formel. |
| [OldFormula](../../aspose.cells.revisions/revisiondefinedname/oldformula/) { get; } | Liest die alte Formel. |
| [Text](../../aspose.cells.revisions/revisiondefinedname/text/) { get; } | Liest den Text des definierten Namens. |
| override [Type](../../aspose.cells.revisions/revisiondefinedname/type/) { get; } | Stellt den Typ der Revision dar. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ermittelt das Arbeitsblatt.(Vererbt von [`Revision`](../revision/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDefinedNameDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Füge einen definierten Namen zum Arbeitsbuch hinzu
                int nameIndex = workbook.Worksheets.Names.Add("TestDefinedName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Ändere den definierten Namen, um eine Revision zu erstellen
                definedName.RefersTo = "=Sheet1!$B$1";

                // Speichere das Arbeitsbuch, um Revisionsprotokolle zu erzeugen
                string filePath = "RevisionDefinedNameDemo.xlsx";
                workbook.Save(filePath);

                // Öffne das Arbeitsbuch erneut, um auf Revisionsinformationen zuzugreifen
                Workbook revisionWorkbook = new Workbook(filePath);

                // Iteriere durch Revisionsprotokolle, um RevisionDefinedName-Einträge zu finden
                foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName revisionDefinedName = (RevisionDefinedName)revision;

                            // Zeige die Eigenschaften von RevisionDefinedName an
                            Console.WriteLine($"Revision Type: {revisionDefinedName.Type}");
                            Console.WriteLine($"Defined Name Text: {revisionDefinedName.Text}");
                            Console.WriteLine($"Old Formula: {revisionDefinedName.OldFormula}");
                            Console.WriteLine($"New Formula: {revisionDefinedName.NewFormula}");
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

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


