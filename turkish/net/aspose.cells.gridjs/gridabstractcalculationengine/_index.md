---
title: "Sınıf GridAbstractCalculationEngine"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridJs.GridAbstractCalculationEngine sınıfı. Kullanıcıların varsayılan Aspose.Cells hesaplama motorunu genişletmek için özel hesaplama motorunu temsil eder"
type: docs
url: /tr/net/aspose.cells.gridjs/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

Kullanıcının, Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel hesaplama motorunu temsil eder.

```csharp
public abstract class GridAbstractCalculationEngine
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridjs/gridabstractcalculationengine/calculate/)(GridCalculationData) | Verilen verilerle bir fonksiyonu hesaplar. |

### Açıklamalar

Kullanıcı, bu uygulamada Çalışma Kitabının herhangi bir bölümünü doğrudan değiştirmemelidir (özel işlevin hesaplanmış sonucu dışındaki, GridCalculationData.CalculatedValue özelliğiyle ayarlanabilen durum hariç). Aksi takdirde beklenmeyen sonuçlar veya İstisna oluşabilir. Kullanıcı, bazı özel işlevler için hesaplanmış sonuç dışındaki diğer verileri değiştirmesi gerekiyorsa, örneğin hücrenin formülünü, stilini vb. değiştirmek istiyorsa, bu verileri bu uygulama içinde toplamalı ve formül hesaplaması kapsamı dışına çıkarak değiştirmelidir.

### Örnekler

```csharp
[C#]
 class MyEngine : GridAbstractCalculationEngine
{
    public override void Calculate(GridCalculationData data)
    {
        string funcName = data.FunctionName.ToUpper();
        if ("MYFUNC".Equals(funcName))
        {   
            //MYFUNC için burada hesaplama yap
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
                //parametreyi burada işleyin
                //res = ...;
            }
            data.CalculatedValue = res;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


