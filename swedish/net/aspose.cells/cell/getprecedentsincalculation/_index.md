---
title: GetPrecedentsInCalculation
second_title: Aspose.Cells för .NET API-referens
description: Hämtar alla prejudikat referens till celler i aktuell arbetsbok som används av denna cells formel när den beräknas.
type: docs
weight: 480
url: /sv/net/aspose.cells/cell/getprecedentsincalculation/
---
## Cell.GetPrecedentsInCalculation method

Hämtar alla prejudikat (referens till celler i aktuell arbetsbok) som används av denna cells formel när den beräknas.

```csharp
public IEnumerator GetPrecedentsInCalculation()
```

### Returvärde

Enumerator för att räkna upp alla referenser (ReferredArea)

### Anmärkningar

Den här metoden kan bara fungera med situationen som[`EnableCalculationChain`](../../formulasettings/enablecalculationchain) är sant för arbetsboken och arbetsboken har beräknats helt. Om den här cellen inte är en formel eller den inte refererar till några andra celler, kommer null att returneras.

### Exempel

```csharp
[C#]

Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["A2"].Formula = "=IF(TRUE,B2,B1)";
workbook.Settings.FormulaSettings.EnableCalculationChain = true;
workbook.CalculateFormula();
IEnumerator en = cells["A2"].GetPrecedentsInCalculation();
Console.WriteLine("A2's calculation precedents:");
while(en.MoveNext())
{
    ReferredArea r = (ReferredArea)en.Current;
    Console.WriteLine(r);
}
```

### Se även

* class [Cell](../../cell)
* namnutrymme [Aspose.Cells](../../cell)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->