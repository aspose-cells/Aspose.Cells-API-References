---
title: "Protection.Password"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Protection property. Représente le mot de passe pour protéger la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/protection/password/
---
## Protection.Password property

Représente le mot de passe pour protéger la feuille de calcul.

```csharp
public string Password { get; set; }
```

### Remarques

Si le mot de passe est défini sur null ou une chaîne vide, vous pouvez déprotéger la feuille de calcul ou le classeur sans utiliser de mot de passe. Sinon, vous devez spécifier le mot de passe pour déprotéger la feuille de calcul ou le classeur.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir les paramètres de protection avec un mot de passe
            Protection protection = worksheet.Protection;
            protection.AllowEditingContent = false;
            protection.AllowDeletingColumn = false;
            protection.Password = "test123";

            // Vérifier la protection par mot de passe
            Console.WriteLine("Worksheet is protected: " + (protection.Password != null));
            Console.WriteLine("Protection password: " + protection.Password);

            // Créer un autre objet de protection pour comparer
            Protection protection2 = worksheet.Protection;
            protection2.Password = "test123";

            // Comparer la protection par mot de passe
            Console.WriteLine("Passwords match: " + (protection.Password == protection2.Password));
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


