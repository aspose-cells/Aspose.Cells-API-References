---
title: Line.IsAuto
second_title: Aspose.Cells for .NET API Reference
description: Line property. Indicates whether this line style is auto assigned
type: docs
url: /net/aspose.cells.drawing/line/isauto/
---
## Line.IsAuto property

Indicates whether this line style is auto assigned.

```csharp
public bool IsAuto { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(ebarSrc.IsAuto, ebarDest.IsAuto, info + ".IsAuto");
public static void Line_Property_IsAuto(ErrorBar ebarSrc, ErrorBar ebarDest, string info)
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
                    AssertHelper.Line_Property_IsAuto(ebarSrc.Color, ebarDest.Color, info + ".Color");
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

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


