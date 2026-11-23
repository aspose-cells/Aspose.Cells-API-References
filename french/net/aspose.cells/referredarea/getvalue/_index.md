---
title: "ReferredArea.GetValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ReferredArea. Obtient la valeur de la cellule avec le décalage donné depuis le coin supérieur gauche de cette zone"
type: docs
url: /fr/net/aspose.cells/referredarea/getvalue/
---
## GetValue(int, int) {#getvalue}

Obtient la valeur de la cellule avec le décalage donné depuis le coin supérieur gauche de cette zone.

```csharp
public object GetValue(int rowOffset, int colOffset)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | décalage de ligne depuis la ligne de départ de cette zone |
| colOffset | Int32 | décalage de colonne depuis la ligne de départ de cette zone |

### Valeur de retour

"#REF!" si cette zone est invalide ; "#N/A" si le décalage donné est hors de cette zone ; sinon retourner la valeur de la cellule à la position donnée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValueWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue(5);
            Cell cell = worksheet.Cells["C1"];
            cell.Formula = "=A1";
            
            workbook.CalculateFormula();
            
            ReferredAreaCollection referredAreas = cell.GetPrecedents();
            if (referredAreas.Count > 0)
            {
                object value = referredAreas[0].GetValue(0, 0);
                Console.WriteLine("Value at (0,0): " + value);
            }
        }
    }
}
```

### Voir aussi

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetValue(int, int, bool) {#getvalue_1}

Obtient la valeur de la cellule avec le décalage donné depuis le coin supérieur gauche de cette zone.

```csharp
public object GetValue(int rowOffset, int colOffset, bool calculateFormulas)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | décalage de ligne depuis la ligne de départ de cette zone |
| colOffset | Int32 | décalage de colonne depuis la ligne de départ de cette zone |
| calculateFormulas | Boolean | Indique s'il faut le calculer de manière récursive si la référence spécifiée est une formule |

### Valeur de retour

"#REF!" si cette zone est invalide ; "#N/A" si le décalage donné est hors de cette zone ; sinon retourner la valeur de la cellule à la position donnée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue(100);
            sheet.Cells["B1"].PutValue(200);

            workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names["TestRange"];
            name.RefersTo = "=Sheet1!$A$1:$B$1";

            ReferredArea ra = name.GetReferredAreas(true)[0];
            object result = ra.GetValue(0, 0, true);

            Console.WriteLine("Obtained value: " + result);
        }
    }
}
```

### Voir aussi

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


