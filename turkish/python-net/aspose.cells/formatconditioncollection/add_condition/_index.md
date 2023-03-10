---
title: add_condition yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 40
url: /tr/python-net/aspose.cells/formatconditioncollection/add_condition/
is_root: false
---
##  add_condition(type) {#FormatConditionType}
Bir biçim koşulu ekleyin.


###  İadeler

Biçimlendirme koşulu nesne dizini;


```python
def add_condition(self, type):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| type | [FormatConditionType](/cells/tr/python-net/aspose.cells/formatconditiontype) | Biçim koşulu türü.|


##  add_condition(type, operator_type, formula1, formula2) {#FormatConditionType-OperatorType-str-str}
Bir biçimlendirme koşulu ekler.


###  İadeler

Biçimlendirme koşulu nesne dizini;


```python
def add_condition(self, type, operator_type, formula1, formula2):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| type | [FormatConditionType](/cells/tr/python-net/aspose.cells/formatconditiontype) | [FormatConditionType](/cells/tr/python-net/aspose.cells/formatconditiontype) koşullu biçimlendirme.<br/> FormatConditionType üyelerinden biri olabilir.|
| operator_type | [OperatorType](/cells/tr/python-net/aspose.cells/operatortype) | Karşılaştırma [OperatorType](/cells/tr/python-net/aspose.cells/operatortype).<br/> OperatorType üyelerinden biri olabilir.|
| formula1 | str | Koşullu biçimlendirmeyle ilişkili değer veya ifade.<br/>Girilen değer '=' ile başlıyorsa, formül olarak alınacaktır.<br/>Aksi takdirde düz değer(metin, sayı, bool) olarak alınacaktır.<br/> '=' ile başlayan metin değeri için, kullanıcı bunu şu biçimde formül olarak girebilir: "=\"=...\"".|
| formula2 | str | Koşullu biçimlendirmeyle ilişkili değer veya ifade.<br/>Giriş formatı, formül1 ile aynıdır|



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [FormatConditionCollection](/cells/tr/python-net/aspose.cells/formatconditioncollection)
* sınıf [FormatConditionType](/cells/tr/python-net/aspose.cells/formatconditiontype)
* sınıf [OperatorType](/cells/tr/python-net/aspose.cells/operatortype)
