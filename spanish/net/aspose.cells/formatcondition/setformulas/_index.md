---
title: "FormatCondition.SetFormulas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FormatCondition. Establece el valor o expresión asociado con esta condición de formato"
type: docs
url: /es/net/aspose.cells/formatcondition/setformulas/
---
## FormatCondition.SetFormulas method

Establece el valor o expresión asociado a esta condición de formato.

```csharp
public void SetFormulas(string formula1, string formula2, bool isR1C1, bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula1 | String | El valor o expresión asociado con esta condición de formato. Si el valor de entrada comienza con '=', se tomará como fórmula. De lo contrario se tomará como valor simple (texto, número, bool). Para valores de texto que comienzan con '=', el usuario puede ingresarlo como fórmula en el formato: "=\"=...\"". |
| formula2 | String | El valor o expresión asociado a esta condición de formato. El formato de entrada es el mismo que formula1 |
| isR1C1 | Booleano | Si la fórmula es una fórmula R1C1. |
| isLocal | Booleano | Si la fórmula está formateada según la configuración regional. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionMethodSetFormulasWithStringStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int formatIndex = cfs.Add();
            FormatConditionCollection fcs = cfs[formatIndex];
            
            fcs.AddArea(CellArea.CreateCellArea("A1", "C10"));
            
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcs[conditionIndex];
            
            fc.Operator = OperatorType.Between;
            fc.SetFormulas("=1", "=2", false, false);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


