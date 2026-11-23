---
title: "Protection.AllowFormattingRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Protection property. Représente si le formatage des lignes est autorisé sur une feuille de calcul protégée"
type: docs
url: /fr/net/aspose.cells/protection/allowformattingrow/
---
## Protection.AllowFormattingRow property

Représente si le formatage des lignes est autorisé sur une feuille de calcul protégée

```csharp
public bool AllowFormattingRow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Activer la protection de la feuille
            worksheet.Protect(ProtectionType.All);

            // Accéder aux paramètres de protection
            Protection protection = worksheet.Protection;

            // Autoriser le formatage des lignes tout en conservant les autres protections
            protection.AllowFormattingRow = true;

            // Enregistrez le classeur
            workbook.Save("Protection_AllowFormattingRow.xlsx");
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


