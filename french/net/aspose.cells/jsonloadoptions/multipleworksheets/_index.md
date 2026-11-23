---
title: "JsonLoadOptions.MultipleWorksheets"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonLoadOptions. Indique si chaque attribut de l'objet JsonObject est importé comme une feuille de calcul lorsque tous les nœuds enfants sont des nœuds de tableau"
type: docs
url: /fr/net/aspose.cells/jsonloadoptions/multipleworksheets/
---
## JsonLoadOptions.MultipleWorksheets property

Indique s'il faut importer chaque attribut de l'objet JsonObject comme une feuille de calcul lorsque tous les nœuds enfants sont des nœuds de tableau.

```csharp
public bool MultipleWorksheets { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyMultipleWorksheetsDemo
    {
        public static void Run()
        {
            // Créer des options de chargement JSON avec MultipleWorksheets activé
            JsonLoadOptions options = new JsonLoadOptions { MultipleWorksheets = true };
            
            // Charger le fichier JSON dans le classeur avec les options spécifiées
            Workbook workbook = new Workbook("example.json", options);
            
            // Accéder aux données de la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Afficher quelques valeurs d'exemple du JSON chargé
            Console.WriteLine("D5 cell value: " + cells["D5"].StringValue);
            Console.WriteLine("E5 cell value: " + cells["E5"].StringValue);
            Console.WriteLine("D7 cell value: " + cells["D7"].StringValue);
            Console.WriteLine("B14 cell value: " + cells["B14"].StringValue);
        }
    }
}
```

### Voir aussi

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


