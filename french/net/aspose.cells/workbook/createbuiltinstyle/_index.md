---
title: "Workbook.CreateBuiltinStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Crée un style intégré selon le type donné"
type: docs
url: /fr/net/aspose.cells/workbook/createbuiltinstyle/
---
## Workbook.CreateBuiltinStyle method

Crée un style intégré selon le type donné.

```csharp
public Style CreateBuiltinStyle(BuiltinStyleType type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | BuiltinStyleType | Le style intégré. |

### Valeur de retour

[`Style`](../../style/) object

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateBuiltinStyleWithBuiltinStyleTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Appliquer le style intégré Good
            workbook.Worksheets[0].Cells["A1"].PutValue("Good");
            Style goodStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Good);
            workbook.Worksheets[0].Cells["A1"].SetStyle(goodStyle);
            
            // Appliquer le style intégré Neutral
            workbook.Worksheets[0].Cells["B2"].PutValue("Neutral");
            Style neutralStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Neutral);
            workbook.Worksheets[0].Cells["B2"].SetStyle(neutralStyle);
            
            // Enregistrez le classeur
            workbook.Save("BuiltinStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* enum [BuiltinStyleType](../../builtinstyletype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


