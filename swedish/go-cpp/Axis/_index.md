---
title: "Axelklass"
linktitle: "Axel"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Axelklass. Inkapslar objektet som representerar en axel i Go."
type: docs
weight: 200
url: /sv/go-cpp/axis/
---

## Axis class

Inkapslar objektet som representerar en axel i ett diagram.

```go

type Axis struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetArea](./getarea/) | Hämtar området. |
| [IsAutomaticMinValue](./isautomaticminvalue/) | Anger om minvärdet tilldelas automatiskt. |
| [SetIsAutomaticMinValue](./setisautomaticminvalue/) | Anger om minvärdet tilldelas automatiskt. |
| [GetMinValue](./getminvalue/) | Representerar minsta värdet på värdeaxeln. |
| [SetMinValue](./setminvalue/) | Representerar minsta värdet på värdeaxeln. |
| [IsAutomaticMaxValue](./isautomaticmaxvalue/) | Anger om maxvärdet tilldelas automatiskt. |
| [SetIsAutomaticMaxValue](./setisautomaticmaxvalue/) | Anger om maxvärdet tilldelas automatiskt. |
| [GetMaxValue](./getmaxvalue/) | Representerar största värdet på värdeaxeln. |
| [SetMaxValue](./setmaxvalue/) | Representerar största värdet på värdeaxeln. |
| [IsAutomaticMajorUnit](./isautomaticmajorunit/) | Anger om huvudenheten för axeln tilldelas automatiskt. |
| [SetIsAutomaticMajorUnit](./setisautomaticmajorunit/) | Anger om huvudenheten för axeln tilldelas automatiskt. |
| [GetMajorUnit](./getmajorunit/) | Representerar huvudenheterna för axeln. |
| [SetMajorUnit](./setmajorunit/) | Representerar huvudenheterna för axeln. |
| [IsAutomaticMinorUnit](./isautomaticminorunit/) | Anger om underenheten för axeln tilldelas automatiskt. |
| [SetIsAutomaticMinorUnit](./setisautomaticminorunit/) | Anger om underenheten för axeln tilldelas automatiskt. |
| [GetMinorUnit](./getminorunit/) | Representerar de mindre enheterna för axeln. |
| [SetMinorUnit](./setminorunit/) | Representerar de mindre enheterna för axeln. |
| [GetAxisLine](./getaxisline/) | Hämtar utseendet på en axel. |
| [GetMajorTickMark](./getmajortickmark/) | Representerar typen av huvudstapelflagga för den angivna axeln. |
| [SetMajorTickMark](./setmajortickmark/) | Representerar typen av huvudstapelflagga för den angivna axeln. |
| [GetMinorTickMark](./getminortickmark/) | Representerar typen av mindre stapelflagga för den angivna axeln. |
| [SetMinorTickMark](./setminortickmark/) | Representerar typen av mindre stapelflagga för den angivna axeln. |
| [GetTickLabelPosition](./getticklabelposition/) | Representerar positionen för stapelflaggeetiketter på den angivna axeln. |
| [SetTickLabelPosition](./setticklabelposition/) | Representerar positionen för stapelflaggeetiketter på den angivna axeln. |
| [GetCrossAt](./getcrossat/) | Representerar punkten på värdeaxeln där kategoriaxeln korsar den. |
| [SetCrossAt](./setcrossat/) | Representerar punkten på värdeaxeln där kategoriaxeln korsar den. |
| [GetCrossType](./getcrosstype/) | Representerar CrossType på den angivna axeln där den andra axeln korsar. |
| [SetCrossType](./setcrosstype/) | Representerar CrossType på den angivna axeln där den andra axeln korsar. |
| [GetLogBase](./getlogbase/) | Representerar den logaritmiska basen. Standardvärdet är 10. |
| [SetLogBase](./setlogbase/) | Representerar den logaritmiska basen. Standardvärdet är 10. |
| [IsLogarithmic](./islogarithmic/) | Representerar om skalan för värdeaxeln är logaritmisk eller inte. |
| [SetIsLogarithmic](./setislogarithmic/) | Representerar om skalan för värdeaxeln är logaritmisk eller inte. |
| [IsPlotOrderReversed](./isplotorderreversed/) | Representerar om Microsoft Excel ritar datapunkter från sista till första. |
| [SetIsPlotOrderReversed](./setisplotorderreversed/) | Representerar om Microsoft Excel ritar datapunkter från sista till första. |
| [GetAxisBetweenCategories](./getaxisbetweencategories/) | Representerar om värdeaxeln korsar kategoriaxeln mellan kategorier. |
| [SetAxisBetweenCategories](./setaxisbetweencategories/) | Representerar om värdeaxeln korsar kategoriaxeln mellan kategorier. |
| [GetTickLabels](./getticklabels/) | Returnerar ett TickLabels-objekt som representerar stapelflaggeetiketterna för den angivna axeln. |
| [GetTickLabelSpacing](./getticklabelspacing/) | Representerar antalet kategorier eller serier mellan stapelflaggeetiketter. Gäller endast för kategori- och serieaxlar. |
| [SetTickLabelSpacing](./setticklabelspacing/) | Representerar antalet kategorier eller serier mellan stapelflaggeetiketter. Gäller endast för kategori- och serieaxlar. |
| [IsAutoTickLabelSpacing](./isautoticklabelspacing/) | Indikerar om avståndet mellan stapel‑etiketter är automatiskt |
| [SetIsAutoTickLabelSpacing](./setisautoticklabelspacing/) | Indikerar om avståndet mellan stapel‑etiketter är automatiskt |
| [GetTickMarkSpacing](./gettickmarkspacing/) | Returnerar eller anger antalet kategorier eller serier mellan stapelflaggor. Gäller endast för kategori- och serieaxlar. |
| [SetTickMarkSpacing](./settickmarkspacing/) | Returnerar eller anger antalet kategorier eller serier mellan stapelflaggor. Gäller endast för kategori- och serieaxlar. |
| [GetDisplayUnit](./getdisplayunit/) | Representerar enhetsetiketten för den angivna axeln. |
| [SetDisplayUnit](./setdisplayunit/) | Representerar enhetsetiketten för den angivna axeln. |
| [GetCustomDisplayUnit](./getcustomdisplayunit/) | Anger ett anpassat värde för visningsenheten. |
| [SetCustomDisplayUnit](./setcustomdisplayunit/) | Anger ett anpassat värde för visningsenheten. |
| [GetDisplayUnitLabel](./getdisplayunitlabel/) | Representerar en enhetsetikett på en axel i det angivna diagrammet. Enhetsetiketter är användbara för att diagrammera stora värden – till exempel i miljoner eller miljarder. |
| [IsDisplayUnitLabelShown](./isdisplayunitlabelshown/) | Representerar om enhetsetiketten visas på den angivna axeln. |
| [SetIsDisplayUnitLabelShown](./setisdisplayunitlabelshown/) | Representerar om enhetsetiketten visas på den angivna axeln. |
| [GetTitle](./gettitle/) | Hämtar titeln för denna axel i diagrammet. |
| [GetCategoryType](./getcategorytype/) | Representerar typen av kategoriaxel. |
| [SetCategoryType](./setcategorytype/) | Representerar typen av kategoriaxel. |
| [GetBaseUnitScale](./getbaseunitscale/) | Representerar basenhetsskalan för kategoriaxeln. |
| [SetBaseUnitScale](./setbaseunitscale/) | Representerar basenhetsskalan för kategoriaxeln. |
| [GetMajorUnitScale](./getmajorunitscale/) | Representerar huvudenhetsskalan för kategoriaxeln. |
| [SetMajorUnitScale](./setmajorunitscale/) | Representerar huvudenhetsskalan för kategoriaxeln. |
| [GetMinorUnitScale](./getminorunitscale/) | Representerar huvudenhetsskalan för kategoriaxeln. |
| [SetMinorUnitScale](./setminorunitscale/) | Representerar huvudenhetsskalan för kategoriaxeln. |
| [IsVisible](./isvisible/) | Representerar om axeln är synlig. |
| [SetIsVisible](./setisvisible/) | Representerar om axeln är synlig. |
| [GetMajorGridLines](./getmajorgridlines/) | Representerar huvudnätlinjer på en diagramaxel. |
| [GetMinorGridLines](./getminorgridlines/) | Representerar mindre rutnätslinjer på ett diagramaxel. |
| [GetHasMultiLevelLabels](./gethasmultilevellabels/) | Indikerar om etiketterna ska visas som flernivå. |
| [SetHasMultiLevelLabels](./sethasmultilevellabels/) | Indikerar om etiketterna ska visas som flernivå. |
| [GetAxisTexts](./getaxistexts/) | Hämtar axelns etiketter efter anrop av metoden Chart.Calculate(). |
| [GetBins](./getbins/) | Representerar fack på ett diagram (Histogram/Pareto) axel. |
