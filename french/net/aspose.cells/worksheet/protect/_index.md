---
title: "Worksheet.Protect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Protège la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/protect/
---
## Protect(ProtectionType) {#protect}

Protège la feuille de calcul.

```csharp
public void Protect(ProtectionType type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | ProtectionType | Type de protection. |

### Remarques

Cette méthode protège la feuille de calcul sans mot de passe. Elle peut protéger la feuille de calcul dans toutes les versions du fichier Excel.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            
            // Protégez la feuille de calcul avec le type de protection Objects
            sheet.Protect(ProtectionType.Objects);
            
            // Enregistrez le classeur
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Protect(ProtectionType, string, string) {#protect_1}

Protège la feuille de calcul.

```csharp
public void Protect(ProtectionType type, string password, string oldPassword)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | ProtectionType | Type de protection. |
| mot de passe | String | Mot de passe. |
| oldPassword | String | Si la feuille de calcul est déjà protégée par un mot de passe, veuillez fournir l’ancien mot de passe. Sinon, vous pouvez définir une valeur nulle ou une chaîne vide pour ce paramètre. |

### Remarques

Cette méthode peut protéger la feuille de calcul dans toutes les versions du fichier Excel.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeStringStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Protégez la feuille de calcul avec un mot de passe et autorisez tous les types de protection
            worksheet.Protect(ProtectionType.All, "password123", null);
            
            // Enregistrez le classeur
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


