---
title: "Worksheet.Protection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Représente les différents types d'options de protection disponibles pour une feuille de calcul. Prend en charge les options de protection avancées dans ExcelXP et les versions ultérieures."
type: docs
url: /fr/net/aspose.cells/worksheet/protection/
---
## Worksheet.Protection property

Représente les différents types d'options de protection disponibles pour une feuille de calcul. Prend en charge les options de protection avancées dans ExcelXP et les versions ultérieures.

```csharp
public Protection Protection { get; }
```

### Remarques

Cette propriété peut protéger la feuille de calcul dans toutes les versions de fichiers Excel et prendre en charge les options de protection avancées dans ExcelXP et les versions ultérieures.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyProtectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Accéder aux propriétés de protection
            Protection protection = sheet.Protection;
            
            // Définir les propriétés de protection
            protection.AllowEditingObject = false;
            protection.AllowEditingScenario = false;
            
            // Protéger la feuille de calcul (en utilisant la méthode Protect au lieu de définir IsProtectedWithPassword directement)
            sheet.Protect(ProtectionType.All, "password123", null);

            // Enregistrez le classeur
            workbook.Save("WorksheetProtectionDemo.xlsx");

            // Vérifier les paramètres de protection
            Console.WriteLine("AllowEditingObject: " + protection.AllowEditingObject);
            Console.WriteLine("AllowEditingScenario: " + protection.AllowEditingScenario);
        }
    }
}
```

### Voir aussi

* class [Protection](../../protection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


