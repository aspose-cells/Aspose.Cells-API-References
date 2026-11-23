---
title: "DataBarBorder.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "DataBarBorder propriété. Obtient ou définit le type des bordures des barres de données spécifiées par une règle de mise en forme conditionnelle"
type: docs
url: /fr/net/aspose.cells/databarborder/type/
---
## DataBarBorder.Type property

Obtient ou définit le type de la bordure des barres de données spécifiées par une règle de mise en forme conditionnelle.

```csharp
public DataBarBorderType Type { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarBorderPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];

            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(ca);

            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];

            DataBar dataBar = fc.DataBar;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Red;

            workbook.Save("DataBarBorderTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* enum [DataBarBorderType](../../databarbordertype/)
* class [DataBarBorder](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


