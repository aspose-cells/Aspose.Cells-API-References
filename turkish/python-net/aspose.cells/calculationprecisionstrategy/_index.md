---
title: CalculationPrecisionStrategy numaralandırma
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1820
url: /tr/python-net/aspose.cells/calculationprecisionstrategy/
is_root: false
---
##  CalculationPrecisionStrategy numaralandırma
Hesaplama hassasiyetini işlemek için stratejileri numaralandırır.
IEEE 754 Kayan Nokta Aritmetiğinin kesinlik sorunu nedeniyle, bazı "görünüşte basit" formüller beklenen sonuç olarak hesaplanamayabilir.
"=-0.45+0.43+0.02" formülü gibi, işlenenleri doğrudan '+' operatörü ile hesaplarken sonuç sıfır olmaz. Bu tür bir kesinlik sorunu için,
bazı özel stratejiler beklenen sonucu verebilir.



CalculationPrecisionStrategy türü aşağıdaki üyeleri gösterir:

###  alanlar
| Alan| Tanım|
| :- | :- |
| NONE | Hesaplamada strateji uygulanmadı.<br/>Hesaplarken sadece orijinal çift değeri işlenen olarak kullanın ve sonucu doğrudan döndürün.<br/> Performans için en verimli ve çoğu durumda uygulanabilir.|
| ROUND | Hesaplama sonucunu anlamlı basamaklara göre yuvarlar.|
| DECIMAL | Mümkün olduğunda işlenen olarak ondalık kullanır.<br/> Performans için en verimsiz.|



###  Ayrıca bakınız
* modül [aspose.cells](..)
