---
title: "ConditionalFormattingValue.IsGTE"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ConditionalFormattingValue. Obtenez ou définissez le drapeau Greater Than Or Equal. À n'utiliser que pour les ensembles d'icônes, il détermine si cette valeur seuil utilise l'opérateur supérieur ou égal. false indique que supérieur est utilisé au lieu de supérieur ou égal. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/conditionalformattingvalue/isgte/
---
## ConditionalFormattingValue.IsGTE property

Obtenez ou définissez le drapeau Greater Than Or Equal. Utilisez uniquement pour les jeux d'icônes, détermine si cette valeur seuil utilise l'opérateur supérieur ou égal. 'false' indique que 'greater than' est utilisé au lieu de 'greater than or equal to'. La valeur par défaut est true.

```csharp
public bool IsGTE { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyIsGTEDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            ws.Cells["A1"].PutValue(1);
            ws.Cells["A2"].PutValue(2);
            ws.Cells["A3"].PutValue(3);
            ws.Cells["A4"].PutValue(4);
            ws.Cells["A5"].PutValue(5);

            // Ajouter une mise en forme conditionnelle
            int index = ws.ConditionalFormattings.Add();
            FormatConditionCollection fcc = ws.ConditionalFormattings[index];
            fcc.AddArea(CellArea.CreateCellArea("A1", "A5"));

            // Créez un format d'échelle de couleur
            index = fcc.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcc[index];
            
            // Configurez une échelle à 2 couleurs
            fc.ColorScale.Is3ColorScale = false;
            
            // Définissez le format de la valeur maximale (démonstration de IsGTE)
            fc.ColorScale.MaxCfvo.IsGTE = true;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Yellow;
            
            // Définissez le format de la valeur minimale
            fc.ColorScale.MinCfvo.IsGTE = true;
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;

            // Enregistrez le classeur
            workbook.Save("ConditionalFormattingValuePropertyIsGTEDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


