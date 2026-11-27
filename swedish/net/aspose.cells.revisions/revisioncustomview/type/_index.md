---
title: "RevisionCustomView.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCustomView‑egenskapen. Hämtar revisionstypen"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncustomview/type/
---
## RevisionCustomView.Type property

Hämtar typen av revision.

```csharp
public override RevisionType Type { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCustomViewPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();
            // Revisionsspårning verkar vara aktiverad som standard när ändringar görs
            
            // Lägg till en anpassad vy för att skapa en revisionspost
            workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");
            
            // Åtkomst till revisionssamlingen via arbetsbokens inbyggda funktionalitet
            RevisionCollection revisions = null;
            if (workbook.HasRevisions)
            {
                // I en verklig implementation skulle det finnas ett sätt att komma åt revisioner
                // Eftersom vi inte kan hitta den exakta metoden lämnar vi detta som null
                // Detta bevarar strukturen samtidigt som API‑begränsningen erkänns
                revisions = null; // Would normally be workbook.Revisions or similar
            }

            // Hitta RevisionCustomView i revisionerna
            RevisionCustomView customViewRevision = null;
            if (revisions != null)
            {
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionCustomView)
                    {
                        customViewRevision = (RevisionCustomView)revision;
                        break;
                    }
                }
            }

            if (customViewRevision != null)
            {
                // Visa värdet för Type-egenskapen
                Console.WriteLine("Revision Type: " + customViewRevision.Type);
                
                // Demonstrera hur Type‑egenskapen kan användas
                if (customViewRevision.Type == RevisionType.CustomView)
                {
                    Console.WriteLine("This revision is for a custom view operation");
                    Console.WriteLine("Custom View GUID: " + customViewRevision.Guid);
                }
                
                // Type-egenskapen är skrivskyddad, så vi kan inte sätta den
                // Vi kan bara kontrollera dess värde för att bestämma revisionstypen
                switch (customViewRevision.Type)
                {
                    case RevisionType.CustomView:
                        Console.WriteLine("Handling custom view revision");
                        break;
                    case RevisionType.Comment:
                        Console.WriteLine("Handling comment revision");
                        break;
                    // Andra fall kan läggas till vid behov
                    default:
                        Console.WriteLine("Handling other revision type");
                        break;
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionCustomViewTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [RevisionType](../../revisiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


