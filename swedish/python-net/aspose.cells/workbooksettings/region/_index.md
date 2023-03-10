---
title: region fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 520
url: /sv/python-net/aspose.cells/workbooksettings/region/
is_root: false
---
##  region fastighet

Hämtar eller ställer in de regionala inställningarna för arbetsboken.

###  Anmärkningar

1. Regionala inställningar som används av Aspose.Cells-komponenten för en arbetsbok som laddas från mallfilen:
i). För en XLS-fil finns det fält definierade för regionala inställningar och MS Excel sparar regionala inställningar i filen när XLS-filen sparas.
Så vi använder den sparade region i mallfilen för arbetsboken.
Om du inte vill använda region som sparats i filen XLS, vänligen återställ den till den förväntade (som CountryCode.Default) efter att ha laddat mallfilen.
Och vi sparar det användarspecificerade värdet (med den här metoden) i filen också när vi sparar en XLS-fil.
ii). För andra filformat, såsom XLSX, XLSB...etc., finns det inget fält definierat för regionala inställningar i filformatspecifikationen.
Så vi använder de regionala inställningarna för programmets miljö för arbetsboken.
Och det användarspecificerade värdet (med den här metoden) kan inte behållas för de genererade filerna med dessa filformat.
2. För vyeffekten i MS Excel:
De tillämpade regionala inställningarna här kan endast träda i kraft vid körning med Aspose.Cells-komponenten och inte när du visar den genererade filen med MS Excel.
Även för den genererade XLS-filen där de angivna regionala inställningarna har sparats, när du visar/redigerar den med MS Excel,
den använda region för att utföra formatering med MS Excel är alltid de regionala standardinställningarna för miljön där MS Excel körs,
inte den som sparats i filen. Det är MS Excels beteende och kan inte ändras med kod.
###  Definition:
```python
@property
def region(self):
    ...
@region.setter
def region(self, value):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [CountryCode](/cells/sv/python-net/aspose.cells/countrycode)
* klass [WorkbookSettings](/cells/sv/python-net/aspose.cells/workbooksettings)
