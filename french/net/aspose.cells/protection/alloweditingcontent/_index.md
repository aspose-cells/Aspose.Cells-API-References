---
title: "Protection.AllowEditingContent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Protection. Indique si l'utilisateur est autorisé à modifier le contenu des cellules verrouillées sur une feuille de calcul protégée"
type: docs
url: /fr/net/aspose.cells/protection/alloweditingcontent/
---
## Protection.AllowEditingContent property

Représente si l'utilisateur est autorisé à modifier le contenu des cellules verrouillées sur une feuille de calcul protégée.

```csharp
public bool AllowEditingContent { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingContentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Protéger la feuille de calcul avec un mot de passe
            worksheet.Protect(ProtectionType.All, "password", null);
            
            // Vérifier et afficher la propriété AllowEditingContent
            Console.WriteLine("AllowEditingContent before setting: " + worksheet.Protection.AllowEditingContent);
            
            // Modifier la propriété AllowEditingContent
            worksheet.Protection.AllowEditingContent = true;
            
            // Vérifier et afficher la propriété mise à jour
            Console.WriteLine("AllowEditingContent after setting: " + worksheet.Protection.AllowEditingContent);
            
            // Enregistrez le classeur
            workbook.Save("ProtectionPropertyAllowEditingContentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


