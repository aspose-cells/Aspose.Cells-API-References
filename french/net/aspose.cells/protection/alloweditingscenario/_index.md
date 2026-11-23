---
title: "Protection.AllowEditingScenario"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Protection. Représente si l'utilisateur est autorisé à modifier les scénarios sur une feuille protégée"
type: docs
url: /fr/net/aspose.cells/protection/alloweditingscenario/
---
## Protection.AllowEditingScenario property

Représente si l'utilisateur est autorisé à modifier les scénarios sur une feuille de calcul protégée.

```csharp
public bool AllowEditingScenario { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingScenarioDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);

            // Accéder aux paramètres de protection de la feuille de calcul
            Protection protection = worksheet.Protection;

            // Définir les propriétés de protection avec AllowEditingScenario activé
            protection.AllowEditingScenario = true;
            protection.AllowFormattingCell = true;  // Corrected property name
            protection.Password = "password123";

            // Protéger la feuille de calcul
            worksheet.Protect(ProtectionType.All);

            // Enregistrez le classeur
            workbook.Save("ProtectionWithScenarioEditing.xlsx");

            Console.WriteLine("Worksheet protected with AllowEditingScenario enabled.");
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


