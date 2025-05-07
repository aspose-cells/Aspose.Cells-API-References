---
title: ErrorBar.MinusValue
second_title: Aspose.Cells for .NET API Reference
description: ErrorBar property. Represents negative error amount when error bar type is Custom
type: docs
url: /net/aspose.cells.charts/errorbar/minusvalue/
---
## ErrorBar.MinusValue property

Represents negative error amount when error bar type is Custom.

```csharp
public string MinusValue { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(ebarSrc.MinusValue, ebarDest.MinusValue, info + ".MinusValue");
public static void Property_MinusValue(ErrorBar ebarSrc, ErrorBar ebarDest, string info)
        {
            if (AssertHelper.checkNull(ebarSrc, ebarDest, info))
            {
                return;
            }            
            bool isVisibleSrc = ebarSrc.IsVisible;
            bool isVisibleDest = ebarDest.IsVisible;
            AssertHelper.AreEqual(isVisibleSrc, isVisibleDest, info);
            if (isVisibleSrc && isVisibleDest)
            {
                //============compare patterns=====================//
                AssertHelper.AreEqual(ebarSrc.IsAuto, ebarDest.IsAuto, info + ".IsAuto");
                if (ebarSrc.IsAuto == false && ebarDest.IsAuto == false)
                {
                    AssertHelper.AreEqual(ebarSrc.Style, ebarDest.Style, info + ".Style");
                    AssertHelper.Property_MinusValue(ebarSrc.Color, ebarDest.Color, info + ".Color");
                    AssertHelper.AreEqual(ebarSrc.Weight, ebarDest.Weight, info + ".Weight");
                }
                AssertHelper.AreEqual(ebarSrc.ShowMarkerTTop, ebarDest.ShowMarkerTTop, info + ".ShowMarkerTTop");
                //=============compare errorbars===================//
                AssertHelper.AreEqual(ebarSrc.DisplayType, ebarDest.DisplayType, info + ".DisplayType");
                AssertHelper.AreEqual(ebarSrc.Type, ebarDest.Type, info + ".Type");
                switch (ebarSrc.Type)
                {
                    case ErrorBarType.FixedValue:
                    case ErrorBarType.Percent:
                    case ErrorBarType.StDev:
                        AssertHelper.AreEqual(ebarSrc.Amount, ebarDest.Amount, info + ".Amount");
                        break;
                    case ErrorBarType.Custom:
                        AssertHelper.AreEqual(ebarSrc.MinusValue, ebarDest.MinusValue, info + ".MinusValue");
                        AssertHelper.AreEqual(ebarSrc.PlusValue, ebarDest.PlusValue, info + ".PlusValue");
                        break;                   
                }
            }

        }
```

### See Also

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


