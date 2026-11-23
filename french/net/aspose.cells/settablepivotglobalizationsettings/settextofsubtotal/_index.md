---
title: "SettablePivotGlobalizationSettings.SetTextOfSubTotal"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettablePivotGlobalizationSettings. Définit le texte du type PivotFieldSubtotalType dans le PivotTable"
type: docs
url: /fr/net/aspose.cells/settablepivotglobalizationsettings/settextofsubtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfSubTotal method

Définit le texte du type [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) dans le PivotTable.

```csharp
public void SetTextOfSubTotal(PivotFieldSubtotalType subTotalType, string text)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | Le [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |
| texte | String | Le texte du type donné |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfSubTotalWithPivotFieldSubtoStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur (juste à des fins de démonstration)
            Workbook workbook = new Workbook();

            // Instance de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Définir un texte personnalisé pour le sous-total Somme
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Sum, "Custom Sum Total");

                // Vérifier le changement
                string sumText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal text after change: {sumText}");

                // Définir un texte personnalisé pour le sous-total Moyenne
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Average, "Custom Average Total");

                // Vérifier le changement
                string avgText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average);
                Console.WriteLine($"Average subtotal text after change: {avgText}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfSubTotal: {ex.Message}");
            }

            // Enregistrer le classeur (aucune modification du tableau croisé dynamique dans cette démo)
            workbook.Save("SetTextOfSubTotalDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


