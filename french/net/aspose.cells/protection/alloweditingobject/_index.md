---
title: "Protection.AllowEditingObject"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Protection. Représente si l'utilisateur est autorisé à manipuler les objets de dessin sur une feuille protégée"
type: docs
url: /fr/net/aspose.cells/protection/alloweditingobject/
---
## Protection.AllowEditingObject property

Représente si l'utilisateur est autorisé à manipuler les objets de dessin sur une feuille de calcul protégée.

```csharp
public bool AllowEditingObject { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir les paramètres de protection avec AllowEditingObject activé
            Protection protection = worksheet.Protection;
            protection.AllowEditingObject = true;
            protection.AllowEditingContent = false; // Contrast with AllowEditingObject
            worksheet.Protect(ProtectionType.All);

            // Vérifier les indicateurs de protection
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowEditingObject: {protection.AllowEditingObject}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // Créer une zone de texte (objet) pour tester la modification
            worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Enregistrez le classeur
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


