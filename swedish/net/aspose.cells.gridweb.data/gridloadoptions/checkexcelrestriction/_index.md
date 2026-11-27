---
title: "GridLoadOptions.CheckExcelRestriction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridLoadOptions‑egenskap. Anger om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att en strängvärde längre än 32 KB matas in. När du matar in ett värde längre än 32 KB, t.ex. via Cell.PutValuestring, får du ett undantag om denna egenskap är true. Om egenskapen är false accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan skriva ut hela strängvärdet för andra filformat som CSV. Däremot bör du inte spara arbetsboken som Excel‑format senare om du har angett ett värde som är ogiltigt för Excel‑formatet. Annars kan det uppstå oväntade fel i den genererade Excel‑filen."
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/
---
## GridLoadOptions.CheckExcelRestriction property

Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att en strängvärde längre än 32 K matas in. När du matar in ett värde längre än 32 K, t.ex. med Cell.PutValue(string), får du ett undantag om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera hela strängvärdet till andra filformat som CSV. Däremot, om du har angett ett värde som är ogiltigt för Excel-filformatet bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Se även

* class [GridLoadOptions](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


