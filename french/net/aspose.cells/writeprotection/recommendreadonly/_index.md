---
title: "WriteProtection.RecommendReadOnly"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WriteProtection. Indique si l'option Lire uniquement recommandé est sélectionnée"
type: docs
url: /fr/net/aspose.cells/writeprotection/recommendreadonly/
---
## WriteProtection.RecommendReadOnly property

Indique si l’option Lecture seule recommandée est sélectionnée.

```csharp
public bool RecommendReadOnly { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyRecommendReadOnlyDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la feuille de calcul et ajouter des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Définir RecommendReadOnly sur true
            workbook.Settings.WriteProtection.RecommendReadOnly = true;
            
            // Vérifier que la propriété est définie
            Console.WriteLine("RecommendReadOnly: " + workbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("IsWriteProtected: " + workbook.Settings.WriteProtection.IsWriteProtected);

            // Enregistrez le classeur
            workbook.Save("output_recommend_readonly.xlsx");

            // Charger le classeur enregistré pour vérifier que les paramètres persistent
            Workbook loadedWorkbook = new Workbook("output_recommend_readonly.xlsx");
            Console.WriteLine("After loading - RecommendReadOnly: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("After loading - IsWriteProtected: " + loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### Voir aussi

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


