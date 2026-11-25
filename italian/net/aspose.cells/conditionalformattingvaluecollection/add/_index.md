---
title: "ConditionalFormattingValueCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ConditionalFormattingValueCollection. Aggiunge l'oggetto ConditionalFormattingValue"
type: docs
url: /it/net/aspose.cells/conditionalformattingvaluecollection/add/
---
## ConditionalFormattingValueCollection.Add method

Aggiunge l'oggetto [`ConditionalFormattingValue`](../../conditionalformattingvalue/).

```csharp
public int Add(FormatConditionValueType type, string value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | FormatConditionValueType | Il tipo di valore. |
| valore | String | Il valore. |

### Valore di ritorno

Restituisce l'indice del nuovo oggetto nell'elenco.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValueCollectionMethodAddWithFormatConditionValueTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[conditionIndex];
            IconSet iconSet = cond.IconSet;
            iconSet.Type = IconSetType.Arrows3;

            ConditionalFormattingValueCollection cfvos = iconSet.Cfvos;
            int cfvIndex = cfvos.Add(FormatConditionValueType.Number, "50");

            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            workbook.Save("ConditionalFormattingValueCollectionExample.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FormatConditionValueType](../../formatconditionvaluetype/)
* class [ConditionalFormattingValueCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


