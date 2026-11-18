---
title: "GetCheckExcelRestriction Metod"
linktitle: "GetCheckExcelRestriction"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "GetCheckExcelRestriction metod. Inkapslar funktionen som representerar getcheckexcelrestriction i Go."
type: docs
weight: 200
url: /sv/go-cpp/abstracttextloadoptions/getcheckexcelrestriction/
---

## GetCheckExcelRestriction function

Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K, till exempel via Cell.PutValue(string), får du ett Undantag om detta egenskap är true. Om egenskapen är false accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera det kompletta strängvärdet till andra filformat såsom CSV. Däremot, om du har angett ett sådant värde som är ogiltigt för Excel-filformatet, bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen.

```go

func (instance *AbstractTextLoadOptions) GetCheckExcelRestriction()  (bool,  error) 

```

## Anmärkningar


## Se även

* Class [AbstractTextLoadOptions](../)
* Library [Aspose.Cells for Go](../../)
