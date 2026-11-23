---
title: "CustomProperty.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "CustomProperty propriété. Retourne ou définit la valeur de la propriété personnalisée"
type: docs
url: /fr/net/aspose.cells.properties/customproperty/value/
---
## CustomProperty.Value property

Renvoie ou définit la valeur de la propriété personnalisée.

```csharp
public string Value { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une propriété personnalisée avec une valeur de chaîne longue
            worksheet.CustomProperties.Add("VeryLongString", "This is a very long string value for testing custom properties");
            
            // Obtenir et afficher la valeur de la propriété personnalisée
            string propertyValue = worksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Custom Property Value: " + propertyValue);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Recharger le classeur pour vérifier que la propriété persiste
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Vérifier que la valeur est la même après le chargement
            string loadedValue = loadedWorksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Reloaded Custom Property Value: " + loadedValue);
        }
    }
}
```

### Voir aussi

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


