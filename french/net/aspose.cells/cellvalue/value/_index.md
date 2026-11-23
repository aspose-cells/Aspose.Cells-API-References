---
title: "CellValue.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellValue. Obtient ou définit la valeur de la cellule"
type: docs
url: /fr/net/aspose.cells/cellvalue/value/
---
## CellValue.Value property

Obtient ou définit la valeur de la cellule.

```csharp
public object Value { get; set; }
```

### Remarques

La valeur doit être du type d'objet correct correspondant à [`Type`](../type/):

| **Type** | **Value** |
| --- | --- |
| IsNull | null, tout autre objet sera ignoré |
| IsNumeric | double |
| IsDateTime | DateTime |
| IsString | string |
| IsBool | bool |
| IsError | chaîne d'erreur telle que "#VALUE!", "#NAME?", ... |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellValuePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CellValue cellValue = new CellValue();
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            worksheet.Cells["A1"].PutValue(cellValue.Value);

            workbook.Save("CellValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


