---
title: "Trendline-klass"
linktitle: "Trendline"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Trendline-klass. Inkapslar objektet som representerar trendline i Go."
type: docs
weight: 200
url: /sv/go-cpp/trendline/
---

## Trendline class

Representerar en trendlinje i ett diagram.

```go

type Trendline struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewTrendline](./newtrendline/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [IsNameAuto](./isnameauto/) | Returnerar om Microsoft Excel automatiskt bestämmer namnet på trendlinjen. |
| [SetIsNameAuto](./setisnameauto/) | Returnerar om Microsoft Excel automatiskt bestämmer namnet på trendlinjen. |
| [GetType](./gettype/) | Returnerar trendlinjetypen. |
| [GetName](./getname/) | Returnerar namnet på trendlinjen. |
| [SetName](./setname/) | Returnerar namnet på trendlinjen. |
| [GetOrder](./getorder/) | Returnerar eller anger trendlinjens ordning (ett heltal större än 1) när trendlinjetypen är Polynomial. Ordningen måste vara mellan 2 och 6. |
| [SetOrder](./setorder/) | Returnerar eller anger trendlinjens ordning (ett heltal större än 1) när trendlinjetypen är Polynomial. Ordningen måste vara mellan 2 och 6. |
| [GetPeriod](./getperiod/) | Returnerar eller anger perioden för den glidande medelvärdestrendlinjen. |
| [SetPeriod](./setperiod/) | Returnerar eller anger perioden för den glidande medelvärdestrendlinjen. |
| [GetForward](./getforward/) | Returnerar eller anger antalet perioder (eller enheter på ett spridningsdiagram) som trendlinjen sträcker sig framåt. Antalet perioder måste vara större än eller lika med noll. |
| [SetForward](./setforward/) | Returnerar eller anger antalet perioder (eller enheter på ett spridningsdiagram) som trendlinjen sträcker sig framåt. Antalet perioder måste vara större än eller lika med noll. |
| [GetBackward](./getbackward/) | Returnerar eller anger antalet perioder (eller enheter på ett spridningsdiagram) som trendlinjen sträcker sig bakåt. Antalet perioder måste vara större än eller lika med noll. Om diagramtypen är stapel måste antalet perioder vara mellan 0 och 0,5 |
| [SetBackward](./setbackward/) | Returnerar eller anger antalet perioder (eller enheter på ett spridningsdiagram) som trendlinjen sträcker sig bakåt. Antalet perioder måste vara större än eller lika med noll. Om diagramtypen är stapel måste antalet perioder vara mellan 0 och 0,5 |
| [GetDisplayEquation](./getdisplayequation/) | Anger om ekvationen för trendlinjen visas i diagrammet (i samma datamärkning som R‑kvadrerat‑värdet). Att sätta denna egenskap till True aktiverar automatiskt datamärkningar. |
| [SetDisplayEquation](./setdisplayequation/) | Anger om ekvationen för trendlinjen visas i diagrammet (i samma datamärkning som R‑kvadrerat‑värdet). Att sätta denna egenskap till True aktiverar automatiskt datamärkningar. |
| [GetDisplayRSquared](./getdisplayrsquared/) | Anger om R‑kvadrerat‑värdet för trendlinjen visas i diagrammet (i samma datamärkning som ekvationen). Att sätta denna egenskap till True aktiverar automatiskt datamärkningar. |
| [SetDisplayRSquared](./setdisplayrsquared/) | Anger om R‑kvadrerat‑värdet för trendlinjen visas i diagrammet (i samma datamärkning som ekvationen). Att sätta denna egenskap till True aktiverar automatiskt datamärkningar. |
| [GetIntercept](./getintercept/) | Returnerar eller anger punkten där trendlinjen korsar värdeaxeln. |
| [SetIntercept](./setintercept/) | Returnerar eller anger punkten där trendlinjen korsar värdeaxeln. |
| [GetDataLabels](./getdatalabels/) | Representerar DataLabels‑objektet för den angivna serien. |
| [GetLegendEntry](./getlegendentry/) | Hämtar förklaringsposten för denna trendlinje |
| [GetCompoundType](./getcompoundtype/) | Anger den sammansatta linjetypen |
| [SetCompoundType](./setcompoundtype/) | Anger den sammansatta linjetypen |
| [GetDashType](./getdashtype/) | Anger strecklinjetypen |
| [SetDashType](./setdashtype/) | Anger strecklinjetypen |
| [GetCapType](./getcaptype/) | Anger avslutningsändarna |
| [SetCapType](./setcaptype/) | Anger avslutningsändarna |
| [GetJoinType](./getjointype/) | Anger sammanfogningsändarna |
| [SetJoinType](./setjointype/) | Anger sammanfogningsändarna |
| [GetBeginType](./getbegintype/) | Anger ett pilhuvud för början av en linje |
| [SetBeginType](./setbegintype/) | Anger ett pilhuvud för början av en linje |
| [GetEndType](./getendtype/) | Anger ett pilhuvud för slutet av en linje |
| [SetEndType](./setendtype/) | Anger ett pilhuvud för slutet av en linje |
| [GetBeginArrowLength](./getbeginarrowlength/) | Anger längden på pilhuvudet för början av en linje |
| [SetBeginArrowLength](./setbeginarrowlength/) | Anger längden på pilhuvudet för början av en linje |
| [GetEndArrowLength](./getendarrowlength/) | Anger längden på pilhuvudet för slutet av en linje |
| [SetEndArrowLength](./setendarrowlength/) | Anger längden på pilhuvudet för slutet av en linje |
| [GetBeginArrowWidth](./getbeginarrowwidth/) | Anger bredden på pilhuvudet för början av en linje |
| [SetBeginArrowWidth](./setbeginarrowwidth/) | Anger bredden på pilhuvudet för början av en linje |
| [GetEndArrowWidth](./getendarrowwidth/) | Anger bredden på pilhuvudet för slutet av en linje |
| [SetEndArrowWidth](./setendarrowwidth/) | Anger bredden på pilhuvudet för slutet av en linje |
| [GetThemeColor](./getthemecolor/) | Hämtar och anger temafärgen. |
| [SetThemeColor](./setthemecolor/) | Hämtar och anger temafärgen. |
| [GetColor](./getcolor/) | Representerar färgen på linjen |
| [SetColor](./setcolor/) | Representerar färgen på linjen |
| [GetTransparency](./gettransparency/) | Returnerar eller anger graden av transparens för linjen som ett värde från 0.0 (opak) till 1.0 (klar). |
| [SetTransparency](./settransparency/) | Returnerar eller anger graden av transparens för linjen som ett värde från 0.0 (opak) till 1.0 (klar). |
| [GetStyle](./getstyle/) | Representerar linjens stil |
| [SetStyle](./setstyle/) | Representerar linjens stil |
| [GetWeight](./getweight/) | Hämtar eller anger WeightType för linjen. |
| [SetWeight](./setweight/) | Hämtar eller anger WeightType för linjen. |
| [GetWeightPt](./getweightpt/) | Hämtar eller anger vikten på linjen i enheter av punkter. |
| [SetWeightPt](./setweightpt/) | Hämtar eller anger vikten på linjen i enheter av punkter. |
| [GetWeightPx](./getweightpx/) | Hämtar eller anger vikten på linjen i enheter av pixlar. |
| [SetWeightPx](./setweightpx/) | Hämtar eller anger vikten på linjen i enheter av pixlar. |
| [GetFormattingType](./getformattingtype/) | Hämtar eller anger formattyp. |
| [SetFormattingType](./setformattingtype/) | Hämtar eller anger formattyp. |
| [IsAutomaticColor](./isautomaticcolor/) | Indikerar om linjens färg tilldelas automatiskt. |
| [IsVisible](./isvisible/) | Representerar om linjen är synlig. |
| [SetIsVisible](./setisvisible/) | Representerar om linjen är synlig. |
| [IsAuto](./isauto/) | Indikerar om den här linjestilen tilldelas automatiskt. |
| [SetIsAuto](./setisauto/) | Indikerar om den här linjestilen tilldelas automatiskt. |
| [GetGradientFill](./getgradientfill/) | Representerar gradientfyllning. |
