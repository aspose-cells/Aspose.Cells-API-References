---
title: "Name.RefersTo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Name. Renvoie ou définit la formule à laquelle le nom est défini pour se référer, commençant par un signe égal"
type: docs
url: /fr/net/aspose.cells/name/refersto/
---
## Name.RefersTo property

Renvoie ou définit la formule à laquelle le nom fait référence, commençant par un signe égal.

```csharp
public string RefersTo { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyRefersToDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "Sheet1";

            // Ajouter des plages nommées avec RefersTo
            int index1 = workbook.Worksheets.Names.Add("NamedRange1");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$6:$8";
            
            int index2 = workbook.Worksheets.Names.Add("NamedRange2");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$C:$D";

            // Afficher la propriété RefersTo des plages nommées
            Console.WriteLine("NamedRange1 RefersTo: " + workbook.Worksheets.Names[0].RefersTo);
            Console.WriteLine("NamedRange2 RefersTo: " + workbook.Worksheets.Names[1].RefersTo);
        }
    }
}
```

### Voir aussi

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


