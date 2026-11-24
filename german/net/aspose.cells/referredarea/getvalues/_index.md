---
title: "ReferredArea.GetValues"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReferredArea-Methode. Ruft Zellwerte in diesem Bereich ab."
type: docs
url: /de/net/aspose.cells/referredarea/getvalues/
---
## GetValues() {#getvalues}

Ermittelt Zellwerte in diesem Bereich.

```csharp
public object GetValues()
```

### Rückgabewert

Wenn dieser Bereich ungültig ist, wird "#REF!" zurückgegeben; ist dieser Bereich eine einzelne Zelle, wird das Zellenwertobjekt zurückgegeben; andernfalls wird ein zweidimensionales Array mit allen Werten dieses Bereichs zurückgegeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Collections;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["B1"].PutValue(3);
            worksheet.Cells["B2"].PutValue(4);

            Cell formulaCell = worksheet.Cells["C1"];
            formulaCell.Formula = "=SUM(A1:B2)";

            ReferredAreaCollection referredAreas = formulaCell.GetPrecedents();
            if (referredAreas.Count > 0)
            {
                ReferredArea ra = referredAreas[0];
                object vs = ra.GetValues();

                if (vs is Array)
                {
                    object[][] values = (object[][])vs;
                    foreach (object[] row in values)
                    {
                        foreach (object val in row)
                        {
                            Console.WriteLine($"Value: {val}");
                        }
                    }
                }
            }
        }
    }
}
```

### Siehe auch

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetValues(bool) {#getvalues_1}

Ermittelt Zellwerte in diesem Bereich.

```csharp
public object GetValues(bool calculateFormulas)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| calculateFormulas | Boolean | In diesem Bereich, falls einige Formeln noch nicht berechnet wurden, gibt dieses Flag an, ob diese Formeln rekursiv berechnet werden sollen. |

### Rückgabewert

Wenn dieser Bereich ungültig ist, wird "#REF!" zurückgegeben; ist dieser Bereich eine einzelne Zelle, wird das Zellenwertobjekt zurückgegeben; andernfalls wird ein zweidimensionales Array mit allen Werten dieses Bereichs zurückgegeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValuesWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            string formula = "=A1:B2";
            Cell cell = worksheet.Cells["C1"];
            cell.Formula = formula;

            workbook.CalculateFormula();
            
            ReferredAreaCollection referredAreasCollection = cell.GetPrecedents();
            ReferredArea[] referredAreas = new ReferredArea[referredAreasCollection.Count];
            for (int i = 0; i < referredAreasCollection.Count; i++)
            {
                referredAreas[i] = referredAreasCollection[i];
            }

            if (referredAreas.Length > 0)
            {
                ReferredArea ra = referredAreas[0];
                
                Console.WriteLine("With headers (true):");
                PrintResult(ra.GetValues(true));
                
                Console.WriteLine("\nWithout headers (false):");
                PrintResult(ra.GetValues(false));
            }
        }

        private static void PrintResult(object result)
        {
            if (result is object[,] multiArray)
            {
                for (int i = 0; i < multiArray.GetLength(0); i++)
                {
                    for (int j = 0; j < multiArray.GetLength(1); j++)
                    {
                        Console.Write(multiArray[i, j] + "\t");
                    }
                    Console.WriteLine();
                }
            }
            else if (result is object[] singleArray)
            {
                Console.WriteLine(string.Join("\t", singleArray));
            }
            else
            {
                Console.WriteLine(result);
            }
        }
    }
}
```

### Siehe auch

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


