---
title: "Name.R1C1RefersTo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Name. Obtient ou définit une référence R1C1 du Name"
type: docs
url: /fr/net/aspose.cells/name/r1c1refersto/
---
## Name.R1C1RefersTo property

Obtient ou définit une référence R1C1 du [`Name`](../).

```csharp
public string R1C1RefersTo { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyR1C1RefersToDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter un nouveau nom à la collection de noms
            int nameIndex = workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names[nameIndex];
            
            // Définir la référence R1C1 pour le nom
            name.R1C1RefersTo = "'Sheet1'!R3C1:R9C4";
            
            // Vérifier que la référence a été définie correctement
            Console.WriteLine("Name refers to: " + name.RefersTo);
            
            // Enregistrez le classeur
            workbook.Save("NamePropertyR1C1RefersToDemo_Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


