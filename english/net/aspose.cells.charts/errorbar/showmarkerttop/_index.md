---
title: ErrorBar.ShowMarkerTTop
second_title: Aspose.Cells for .NET API Reference
description: ErrorBar property. Indicates if formatting error bars with a Ttop
type: docs
url: /net/aspose.cells.charts/errorbar/showmarkerttop/
---
## ErrorBar.ShowMarkerTTop property

Indicates if formatting error bars with a T-top.

```csharp
public bool ShowMarkerTTop { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(ebarSrc.ShowMarkerTTop, ebarDest.ShowMarkerTTop, info + &amp;quot;.ShowMarkerTTop&amp;quot;);
public static void Property_ShowMarkerTTop(ErrorBar ebarSrc, ErrorBar ebarDest, string info)
        {
            if (AssertHelper.checkNull(ebarSrc, ebarDest, info))
            {
                return;
            }            
            bool isVisibleSrc = ebarSrc.IsVisible;
            bool isVisibleDest = ebarDest.IsVisible;
            AssertHelper.AreEqual(isVisibleSrc, isVisibleDest, info);
            if (isVisibleSrc &amp;&amp; isVisibleDest)
            {
                //============compare patterns=====================//
                AssertHelper.AreEqual(ebarSrc.IsAuto, ebarDest.IsAuto, info + &quot;.IsAuto&quot;);
                if (ebarSrc.IsAuto == false &amp;&amp; ebarDest.IsAuto == false)
                {
                    AssertHelper.AreEqual(ebarSrc.Style, ebarDest.Style, info + &quot;.Style&quot;);
                    AssertHelper.Property_ShowMarkerTTop(ebarSrc.Color, ebarDest.Color, info + &quot;.Color&quot;);
                    AssertHelper.AreEqual(ebarSrc.Weight, ebarDest.Weight, info + &quot;.Weight&quot;);
                }
                AssertHelper.AreEqual(ebarSrc.ShowMarkerTTop, ebarDest.ShowMarkerTTop, info + &quot;.ShowMarkerTTop&quot;);
                //=============compare errorbars===================//
                AssertHelper.AreEqual(ebarSrc.DisplayType, ebarDest.DisplayType, info + &quot;.DisplayType&quot;);
                AssertHelper.AreEqual(ebarSrc.Type, ebarDest.Type, info + &quot;.Type&quot;);
                switch (ebarSrc.Type)
                {
                    case ErrorBarType.FixedValue:
                    case ErrorBarType.Percent:
                    case ErrorBarType.StDev:
                        AssertHelper.AreEqual(ebarSrc.Amount, ebarDest.Amount, info + &quot;.Amount&quot;);
                        break;
                    case ErrorBarType.Custom:
                        AssertHelper.AreEqual(ebarSrc.MinusValue, ebarDest.MinusValue, info + &quot;.MinusValue&quot;);
                        AssertHelper.AreEqual(ebarSrc.PlusValue, ebarDest.PlusValue, info + &quot;.PlusValue&quot;);
                        break;                   
                }
            }

        }
```

### See Also

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


