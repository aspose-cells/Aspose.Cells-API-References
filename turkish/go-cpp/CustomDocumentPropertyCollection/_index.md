---
title: "CustomDocumentPropertyCollection Sınıfı"
linktitle: "CustomDocumentPropertyCollection"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "CustomDocumentPropertyCollection sınıfı. Go'da customdocumentpropertycollection'ı temsil eden nesneyi kapsar."
type: docs
weight: 200
url: /tr/go-cpp/customdocumentpropertycollection/
---

## CustomDocumentPropertyCollection class

Özel belge özelliklerinin bir koleksiyonu.

```go

type CustomDocumentPropertyCollection struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewCustomDocumentPropertyCollection](./newcustomdocumentpropertycollection/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [Add_String_String](./add_string_string/) | <b>PropertyType.String</b> veri tipinde yeni bir özel belge özelliği oluşturur. |
| [Add_String_Int](./add_string_int/) | <b>PropertyType.Number</b> veri tipinde yeni bir özel belge özelliği oluşturur. |
| [Add_String_Date](./add_string_date/) | <b>PropertyType.DateTime</b> veri tipinde yeni bir özel belge özelliği oluşturur. |
| [Add_String_Bool](./add_string_bool/) | <b>PropertyType.Boolean</b> veri tipinde yeni bir özel belge özelliği oluşturur. |
| [Add_String_Double](./add_string_double/) | <b>PropertyType.Float</b> veri tipinde yeni bir özel belge özelliği oluşturur. |
| [AddLinkToContent](./addlinktocontent/) | İçeriğe bağlanan yeni bir özel belge özelliği oluşturur. |
| [UpdateLinkedPropertyValue](./updatelinkedpropertyvalue/) | İçeriğe bağlı tüm özel özelliklerin değerlerini günceller (usecell value of linked range to update value of custom property). |
| [UpdateLinkedRange](./updatelinkedrange/) | Özel özelliklere bağlı tüm aralıkları günceller (use the value ofcustom document property to update cell value of linked range). |
| [Get_Int](./get_int/) | İndeks ile bir DocumentProperty nesnesi döndürür. |
| [Contains](./contains/) | Belirtilen ada sahip bir özellik koleksiyonda mevcutsa true döndürür. |
| [IndexOf](./indexof/) | Adına göre bir özelliğin indeksini alır. |
| [Remove](./remove/) | Belirtilen ada sahip bir özelliği koleksiyondan kaldırır. |
| [RemoveAt](./removeat/) | Belirtilen indeksteki bir özelliği kaldırır. |
| [GetCount](./getcount/) | Örnekte bulunan öğe sayısını alır. |
