---
title: "Classe WriteProtection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.WriteProtection. Spécifie les paramètres de protection en écriture pour un classeur"
type: docs
url: /fr/net/aspose.cells/writeprotection/
---
## WriteProtection class

Spécifie les paramètres de protection en écriture pour un classeur.

```csharp
public class WriteProtection
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Author](../../aspose.cells/writeprotection/author/) { get; set; } | Obtient et définit l’auteur. |
| [IsWriteProtected](../../aspose.cells/writeprotection/iswriteprotected/) { get; } | Indique si ce classeur est protégé en écriture. |
| [Password](../../aspose.cells/writeprotection/password/) { get; set; } | Définit le mot de passe de protection pour modifier le fichier. |
| [RecommendReadOnly](../../aspose.cells/writeprotection/recommendreadonly/) { get; set; } | Indique si l’option Lecture seule recommandée est sélectionnée. |

## Méthodes

| Nom | Description |
| --- | --- |
| [ValidatePassword](../../aspose.cells/writeprotection/validatepassword/)(string) | Renvoie vrai si le mot de passe spécifié est identique au mot de passe de protection en écriture avec lequel le fichier a été protégé. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WriteProtectionDemo
    {
        public static void WriteProtectionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;

            // Accéder aux paramètres de protection en écriture
            WriteProtection writeProtection = settings.WriteProtection;

            // Définir l'auteur de la protection en écriture
            writeProtection.Author = "John Doe";

            // Définir le mot de passe pour la protection en écriture
            writeProtection.Password = "password123";

            // Définir l'option de lecture seule recommandée
            writeProtection.RecommendReadOnly = true;

            // Vérifier si le classeur est protégé en écriture
            bool isWriteProtected = writeProtection.IsWriteProtected;
            Console.WriteLine("Is Write Protected: " + isWriteProtected);

            // Valider le mot de passe
            bool isValidPassword = writeProtection.ValidatePassword("password123");
            Console.WriteLine("Is Valid Password: " + isValidPassword);

            // Enregistrez le classeur
            workbook.Save("WriteProtectionExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


