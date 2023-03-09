---
title: check_excel_restriction fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 90
url: /sv/python-net/aspose.cells/htmlloadoptions/check_excel_restriction/
is_root: false
---
##  check_excel_restriction fastighet

Om kontrollera begränsning av excel-fil när användaren ändrar cellrelaterade objekt.
Till exempel tillåter excel inte inmatning av strängvärden som är längre än 32K.
När du matar in ett värde som är längre än 32K, till exempel Cell.PutValue(string), får du ett undantag om den här egenskapen är sann.
Om den här egenskapen är falsk kommer vi att acceptera ditt inmatade strängvärde som cellens värde så att senare
du kan mata ut hela strängvärdet för andra filformat som CSV.
Men om du har angett en sådan typ av värde som är ogiltigt för Excel-filformat,
du bör inte spara arbetsboken som Excel-filformat senare.
###  Definition:
```python
@property
def check_excel_restriction(self):
    ...
@check_excel_restriction.setter
def check_excel_restriction(self, value):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [HtmlLoadOptions](/cells/sv/python-net/aspose.cells/htmlloadoptions)
