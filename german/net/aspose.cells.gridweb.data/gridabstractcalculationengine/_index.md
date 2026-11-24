---
title: "Klasse GridAbstractCalculationEngine"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.GridAbstractCalculationEngine Klasse. Stellt die benutzerdefinierte Berechnungs-Engine des Benutzers dar, um die Standard‑Berechnungs‑Engine von Aspose.Cells zu erweitern."
type: docs
url: /de/net/aspose.cells.gridweb.data/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

Stellt die benutzerdefinierte Berechnungs-Engine des Benutzers dar, um die Standard-Berechnungs-Engine von Aspose.Cells zu erweitern.

```csharp
public abstract class GridAbstractCalculationEngine
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridweb.data/gridabstractcalculationengine/calculate/)(GridCalculationData) | Berechnet eine Funktion mit den angegebenen Daten. |

### Beispiele

```csharp
[C#]
 class MyEngine : GridAbstractCalculationEngine
{
    public override void Calculate(GridCalculationData data)
    {
        string funcName = data.FunctionName.ToUpper();
        if ("MYFUNC".Equals(funcName))
        {
            //Führe hier die Berechnung für MYFUNC durch
            int count = data.ParamCount;
            object res = null;
            for (int i = 0; i < count; i++)
            {
                object pv = data.GetParamValue(i);
                if (pv is GridReferredArea)
                {
                    GridReferredArea ra = (GridReferredArea)pv;
                    pv = ra.GetValue(0, 0);
                }
                //Verarbeite hier den Parameter
                //res = ...;
            }
            data.CalculatedValue = res;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


