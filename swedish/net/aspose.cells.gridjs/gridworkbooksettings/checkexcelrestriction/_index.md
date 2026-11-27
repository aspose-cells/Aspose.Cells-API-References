---
title: "GridWorkbookSettings.CheckExcelRestriction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridWorkbookSettings-egenskap. Anger om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter inte Excel att en strängvärde längre än 32 K matas in. När du matar in ett värde längre än 32 K, exempelvis via Cell.PutValuestring, får du ett undantag om denna egenskap är true. Om egenskapen är false accepterar vi ditt inmatade strängvärde som cellvärde så att du senare kan exportera den kompletta strängen till andra filformat såsom CSV. Dock bör du inte spara arbetsboken som Excel‑filformat senare om du har angett ett värde som är ogiltigt för Excel‑filformatet. Annars kan det uppstå oväntade fel i den genererade Excel‑filen. standard är falskt"
type: docs
url: /sv/net/aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/
---
## GridWorkbookSettings.CheckExcelRestriction property

Anger om begränsningar i Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 KB. När du matar in ett värde längre än 32 KB, t.ex. via Cell.PutValue(string), får du ett undantag om denna egenskap är `true`. Om egenskapen är `false` accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera hela strängen till andra filformat som CSV. Dock, om du har angett ett värde som är ogiltigt för Excel‑filformatet bör du inte spara arbetsboken som Excel‑format senare. Annars kan det uppstå oväntade fel i den genererade Excel‑filen. Standardvärdet är `false`.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Se även

* class [GridWorkbookSettings](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


