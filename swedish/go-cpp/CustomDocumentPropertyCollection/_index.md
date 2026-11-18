---
title: "CustomDocumentPropertyCollection klass"
linktitle: "CustomDocumentPropertyCollection"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "CustomDocumentPropertyCollection klass. Inkapslar objektet som representerar customdocumentpropertycollection i Go."
type: docs
weight: 200
url: /sv/go-cpp/customdocumentpropertycollection/
---

## CustomDocumentPropertyCollection class

En samling av anpassade dokumentegenskaper.

```go

type CustomDocumentPropertyCollection struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewCustomDocumentPropertyCollection](./newcustomdocumentpropertycollection/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [Add_String_String](./add_string_string/) | Skapar en ny anpassad dokumentegenskap av datatypen <b>PropertyType.String</b>. |
| [Add_String_Int](./add_string_int/) | Skapar en ny anpassad dokumentegenskap av datatypen <b>PropertyType.Number</b>. |
| [Add_String_Date](./add_string_date/) | Skapar en ny anpassad dokumentegenskap av datatypen <b>PropertyType.DateTime</b>. |
| [Add_String_Bool](./add_string_bool/) | Skapar en ny anpassad dokumentegenskap av datatypen <b>PropertyType.Boolean</b>. |
| [Add_String_Double](./add_string_double/) | Skapar en ny anpassad dokumentegenskap av datatypen <b>PropertyType.Float</b>. |
| [AddLinkToContent](./addlinktocontent/) | Skapar en ny anpassad dokumentegenskap som länkar till innehåll. |
| [UpdateLinkedPropertyValue](./updatelinkedpropertyvalue/) | Uppdaterar värden för alla anpassade egenskaper som är länkade till innehåll (använd cellvärdet i det länkade området för att uppdatera värdet på den anpassade egenskapen). |
| [UpdateLinkedRange](./updatelinkedrange/) | Uppdaterar alla områden som är länkade till anpassade egenskaper (använd värdet från den anpassade dokumentegenskapen för att uppdatera cellvärdet i det länkade området). |
| [Get_Int](./get_int/) | Returnerar ett DocumentProperty-objekt efter index. |
| [Contains](./contains/) | Returnerar true om en egenskap med det angivna namnet finns i samlingen. |
| [IndexOf](./indexof/) | Hämtar indexet för en egenskap efter namn. |
| [Remove](./remove/) | Tar bort en egenskap med det angivna namnet från samlingen. |
| [RemoveAt](./removeat/) | Tar bort en egenskap på det angivna indexet. |
| [GetCount](./getcount/) | Hämtar antalet element som finns i instansen. |
