---
title: "ErrorCheckType Enum"
linktitle: "ErrorCheckType"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "ErrorCheckType enum. Go dilinde errorchecktype'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/errorchecktype/
---

## ErrorCheckType Enum

Tüm hata kontrol türlerini temsil eder.

```go

type ErrorCheckType int32


```

## Alanlar

| Alan | Açıklama |
| --- | --- |
| [EvaluationError](./evaluationerror/) | Hücreler hataya yol açan formüller içerdiğinde hataları yoksayar. |
| [EmptyCellRef](./emptycellref/) | Formüller boş hücrelere referans verdiğinde hataları yoksayar |
| [NumberStoredAsText](./numberstoredastext/) | Sayılar metin olarak biçimlendirildiğinde veya başında tek tırnak işareti olduğunda hataları yoksayar |
| [InconsistRange](./inconsistrange/) | Formüller bir bölgede belirli hücreleri atladığında hataları yoksayar. |
| [InconsistFormula](./inconsistformula/) | Çalışma sayfanızın bir bölgesindeki formül aynı bölgedeki diğer formüllerden farklı olduğunda hataları yoksayar. |
| [TwoDigitTextYear](./twodigittextyear/) | Formüller, yılları 2 basamakla gösteren metin biçimli hücreler içerdiğinde hataları yoksayar. |
| [UnlockedFormula](./unlockedformula/) | Kilidi açılmış hücreler formül içerdiğinde hataları yoksayar |
| [TableDataValidation](./tabledatavalidation/) | Bir Tablo'daki hücrenin değeri belirtilen Veri Doğrulama kurallarına uymadığında hataları yoksayar |
| [CalculatedColumn](./calculatedcolumn/) | Hücreler hesaplanmış sütun formülünden farklı bir değer içerdiğinde hataları yoksay. |
