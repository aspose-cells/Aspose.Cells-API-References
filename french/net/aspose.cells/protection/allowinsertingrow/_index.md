---
title: "Protection.AllowInsertingRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Protection property. Représente si l'insertion de lignes est autorisée sur une feuille de calcul protégée"
type: docs
url: /fr/net/aspose.cells/protection/allowinsertingrow/
---
## Protection.AllowInsertingRow property

Représente si l'insertion de lignes est autorisée sur une feuille de calcul protégée

```csharp
public bool AllowInsertingRow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder aux paramètres de protection
            Protection protection = worksheet.Protection;

            // Activer l'insertion de lignes en mode protégé
            protection.AllowInsertingRow = true;
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Essayez d'insérer une ligne (cela devrait fonctionner puisque AllowInsertingRow est vrai)
            worksheet.Cells.InsertRow(0);

            // Enregistrez le classeur
            workbook.Save("AllowInsertingRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


