---
title: "FormatConditionCollection.AddCondition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FormatConditionCollection. Ajoute une condition de formatage"
type: docs
url: /fr/net/aspose.cells/formatconditioncollection/addcondition/
---
## AddCondition(FormatConditionType, OperatorType, string, string) {#addcondition_1}

Ajoute une condition de formatage.

```csharp
public int AddCondition(FormatConditionType type, OperatorType operatorType, string formula1, 
    string formula2)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | FormatConditionType | Le type de condition de formatage. |
| operatorType | OperatorType | Le type d'opérateur |
| formula1 | String | Valeur ou expression associée au formatage conditionnel. Si la valeur d'entrée commence par '=', elle sera considérée comme une formule. Sinon, elle sera considérée comme une valeur simple (texte, nombre, booléen). Pour une valeur texte qui commence par '=', l'utilisateur peut la saisir comme formule au format : "=\"=...\"". |
| formula2 | String | Valeur ou expression associée au formatage conditionnel. Le format d'entrée est le même que celui de formula1 |

### Valeur de retour

Indice de l'objet condition de formatage ;

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddConditionWithFormatConditionTypeOperatorTypDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 10;
            ca.StartColumn = 0;
            ca.EndColumn = 10;
            fcs.AddArea(ca);
            
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "-50", "-1");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.Font.Color = Color.Red;
            
            conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "0", "50");
            fc = fcs[conditionIndex];
            fc.Style.Font.Color = Color.Green;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCondition(FormatConditionType) {#addcondition}

Ajouter une condition de format.

```csharp
public int AddCondition(FormatConditionType type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | FormatConditionType | Type de condition de formatage. |

### Valeur de retour

Indice de l'objet condition de formatage ;

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddConditionWithFormatConditionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des conditions de formatage
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[formatIndex];
            
            // Ajouter une plage
            CellArea area = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 5,
                EndColumn = 5
            };
            conditions.AddArea(area);

            // Ajouter des conditions (renvoie un indice entier)
            conditions.AddCondition(FormatConditionType.ColorScale);
            conditions.AddCondition(FormatConditionType.IconSet);
            conditions.AddCondition(FormatConditionType.DataBar);

            workbook.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


