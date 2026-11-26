---
title: "Clase GridAbstractCalculationEngine"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridJs.GridAbstractCalculationEngine. Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells"
type: docs
url: /es/net/aspose.cells.gridjs/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells.

```csharp
public abstract class GridAbstractCalculationEngine
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridjs/gridabstractcalculationengine/calculate/)(GridCalculationData) | Calcula una función con los datos proporcionados. |

### Observaciones

El usuario no debe modificar directamente ninguna parte del Workbook en esta implementación (excepto el resultado calculado de la función personalizada, que puede establecerse mediante la propiedad GridCalculationData.CalculatedValue). De lo contrario, podrían producirse resultados inesperados o una Exception. Si el usuario necesita cambiar datos diferentes al resultado calculado en la implementación para algunas funciones personalizadas, por ejemplo, modificar la fórmula de una celda, el estilo, etc., el usuario debe recopilar esos datos en esta implementación y modificarlos fuera del alcance del cálculo de fórmulas.

### Ejemplos

```csharp
[C#]
 class MyEngine : GridAbstractCalculationEngine
{
    public override void Calculate(GridCalculationData data)
    {
        string funcName = data.FunctionName.ToUpper();
        if ("MYFUNC".Equals(funcName))
        {   
            //realizar cálculo para MYFUNC aquí
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
                //procesar el parámetro aquí
                //res = ...;
            }
            data.CalculatedValue = res;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


