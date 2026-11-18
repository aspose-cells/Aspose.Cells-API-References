---
title: "ConnectionParameter Sınıfı"
linktitle: "ConnectionParameter"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "ConnectionParameter sınıfı. Go'da connectionparameter'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/connectionparameter/
---

## ConnectionParameter class

Harici veri bağlantılarıyla kullanılan parametrelerle ilgili özellikleri belirtir. Parametreler ODBC ve web sorguları için geçerlidir.

```go

type ConnectionParameter struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetSqlType](./getsqltype/) | Parametrenin SQL veri tipi. Yalnızca ODBC kaynakları için geçerlidir. |
| [SetSqlType](./setsqltype/) | Parametrenin SQL veri tipi. Yalnızca ODBC kaynakları için geçerlidir. |
| [GetRefreshOnChange](./getrefreshonchange/) | Parametrenin değerini sağlayan bir hücrenin içeriği değiştiğinde sorgunun otomatik olarak yenilenip yenilenmeyeceğini gösteren bayrak. True ise, dış veri her değişiklikte yeni parametre değeri kullanılarak yenilenir. False ise, dış veri yalnızca kullanıcı tarafından istendiğinde veya başka bir olay (ör. çalışma kitabı açıldığında) yenilemeyi tetiklediğinde yenilenir. |
| [SetRefreshOnChange](./setrefreshonchange/) | Parametrenin değerini sağlayan bir hücrenin içeriği değiştiğinde sorgunun otomatik olarak yenilenip yenilenmeyeceğini gösteren bayrak. True ise, dış veri her değişiklikte yeni parametre değeri kullanılarak yenilenir. False ise, dış veri yalnızca kullanıcı tarafından istendiğinde veya başka bir olay (ör. çalışma kitabı açıldığında) yenilemeyi tetiklediğinde yenilenir. |
| [GetPrompt](./getprompt/) | Parametre için istem dizesi. Dış veriyi yenilemeden önce parametre değerini toplamak için giriş UI'siyle birlikte elektronik tablo kullanıcısına sunulur. Yalnızca parameterType = prompt olduğunda kullanılır. |
| [SetPrompt](./setprompt/) | Parametre için istem dizesi. Dış veriyi yenilemeden önce parametre değerini toplamak için giriş UI'siyle birlikte elektronik tablo kullanıcısına sunulur. Yalnızca parameterType = prompt olduğunda kullanılır. |
| [GetType](./gettype/) | Kullanılan parametre türü. parameterType=value ise, boolean, double, integer veya string değerlerinden biri kullanılacaktır. Bu durumda, yalnızca {boolean, double, integer veya string} öğelerinden birinin belirtilmesi beklenir. |
| [SetType](./settype/) | Kullanılan parametre türü. parameterType=value ise, boolean, double, integer veya string değerlerinden biri kullanılacaktır. Bu durumda, yalnızca {boolean, double, integer veya string} öğelerinden birinin belirtilmesi beklenir. |
| [GetName](./getname/) | Parametrenin adı. |
| [SetName](./setname/) | Parametrenin adı. |
| [GetCellReference](./getcellreference/) | Sorgu parametresi için hangi hücrenin değerinin kullanılacağını belirten hücre referansı. Yalnızca parameterType hücre olduğunda kullanılır. |
| [SetCellReference](./setcellreference/) | Sorgu parametresi için hangi hücrenin değerinin kullanılacağını belirten hücre referansı. Yalnızca parameterType hücre olduğunda kullanılır. |
| [GetValue](./getvalue/) | Sorgu parametresi olarak kullanılacak tam sayı olmayan sayısal değer, tam sayı değeri, string değeri veya Boolean değer. Yalnızca parameterType değer olduğunda kullanılır. |
| [SetValue](./setvalue/) | Sorgu parametresi olarak kullanılacak tam sayı olmayan sayısal değer, tam sayı değeri, string değeri veya Boolean değer. Yalnızca parameterType değer olduğunda kullanılır. |
