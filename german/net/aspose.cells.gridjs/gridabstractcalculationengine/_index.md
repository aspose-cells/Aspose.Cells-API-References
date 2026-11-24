---
title: "Klasse GridAbstractCalculationEngine"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridJs.GridAbstractCalculationEngine Klasse. Stellt die benutzerdefinierte Berechnungs‑Engine dar, um die Standard‑Berechnungs‑Engine von Aspose.Cells zu erweitern."
type: docs
url: /de/net/aspose.cells.gridjs/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

Stellt die benutzerdefinierte Berechnungs-Engine des Benutzers dar, um die Standard-Berechnungs-Engine von Aspose.Cells zu erweitern.

```csharp
public abstract class GridAbstractCalculationEngine
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridjs/gridabstractcalculationengine/calculate/)(GridCalculationData) | Berechnet eine Funktion mit den angegebenen Daten. |

### Hinweise

Der Benutzer sollte keinen Teil des Arbeitsbuchs direkt in dieser Implementierung ändern (außer dem berechneten Ergebnis der benutzerdefinierten Funktion, das über die Eigenschaft GridCalculationData.CalculatedValue festgelegt werden kann). Andernfalls können unerwartete Ergebnisse oder Ausnahmen auftreten. Wenn der Benutzer andere Daten als das berechnete Ergebnis in der Implementierung für einige benutzerdefinierte Funktionen ändern muss, zum Beispiel die Zellformel, den Stil, ...etc., sollte er diese Daten in dieser Implementierung sammeln und sie außerhalb des Bereichs der Formelberechnung ändern.

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

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


