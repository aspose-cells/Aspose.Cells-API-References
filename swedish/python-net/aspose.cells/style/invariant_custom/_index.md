---
title: invariant_custom fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 260
url: /sv/python-net/aspose.cells/style/invariant_custom/
is_root: false
---
##  invariant_custom fastighet

Hämtar den kulturoberoende mönstersträngen för talformat.
Om inget talformat har ställts in för detta objekt, returneras null.
Om talformat är inbyggt kommer mönstersträngen som motsvarar det inbyggda numret att returneras.

###  Anmärkningar

För inbyggda talformat är det returnerade mönsterinnehållet fortfarande kulturberoende,
som, för vissa lokaler returnerar den "m/d/y" och för vissa andra lokaler returnerar den "d/m/y".
Skillnaden från [Style.culture_custom](/cells/sv/python-net/aspose.cells/style#culture_custom) är (det är också vad kulturoberoende betyder):
formatspecifikationerna och separatorerna behålls som standard, t.ex. "/" kommer alltid att användas som datetime-separator
och "y" kommer alltid att användas som "år"-delen oavsett vilket annat specialtecken som används för det specifika språket.
###  Definition:
```python
@property
def invariant_custom(self):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [Style](/cells/sv/python-net/aspose.cells/style)
