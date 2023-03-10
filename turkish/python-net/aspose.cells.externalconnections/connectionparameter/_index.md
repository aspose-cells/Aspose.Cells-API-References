---
title: ConnectionParameter sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 10
url: /tr/python-net/aspose.cells.externalconnections/connectionparameter/
is_root: false
---
##  ConnectionParameter sınıfı
Harici veri bağlantılarıyla kullanılan tüm parametrelerle ilgili özellikleri belirtir
Parametreler ODBC ve web sorguları için geçerlidir.



ConnectionParameter türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [sql_type](/cells/tr/python-net/aspose.cells.externalconnections/connectionparameter/sql_type) | Parametrenin SQL veri türü. Yalnızca ODBC kaynakları için geçerlidir.|
| [refresh_on_change](/cells/tr/python-net/aspose.cells.externalconnections/connectionparameter/refresh_on_change) | Bir sorgunun içeriği değiştiğinde sorgunun otomatik olarak yenilenip yenilenmeyeceğini gösteren bayrak<br/> parametre değeri değişikliklerini sağlayan hücre. Doğruysa, harici veriler yenilenir<br/> her değişiklik olduğunda yeni parametre değerini kullanarak. Yanlışsa, harici veriler<br/> yalnızca kullanıcı tarafından istendiğinde veya başka bir olay yenilemeyi tetiklediğinde (örneğin, çalışma kitabı açıldı) yenilenir.|
| [prompt](/cells/tr/python-net/aspose.cells.externalconnections/connectionparameter/prompt) | Parametre için bilgi istemi dizesi. Elektronik tablo kullanıcısına giriş kullanıcı arabirimiyle birlikte sunulur<br/> harici verileri yenilemeden önce parametre değerini toplamak için. Sadece ne zaman kullanılır<br/>parametreTürü = bilgi istemi.|
| [type](/cells/tr/python-net/aspose.cells.externalconnections/connectionparameter/type) | Kullanılan parametre türü.<br/> parameterType=value ise, boolean, double, integer'dan gelen değer,<br/> veya dize kullanılacaktır. Bu durumda, yalnızca birinin olması beklenir.<br/> {boolean, double, integer veya string} belirtilecektir.|
| [name](/cells/tr/python-net/aspose.cells.externalconnections/connectionparameter/name) | Parametrenin adı.|
| [cell_reference](/cells/tr/python-net/aspose.cells.externalconnections/connectionparameter/cell_reference) | Cell sorgu parametresi için hangi hücrenin değerinin kullanılacağını gösteren referans. Yalnızca parameterType hücre olduğunda kullanılır.|
| [value](/cells/tr/python-net/aspose.cells.externalconnections/connectionparameter/value) | Tamsayı olmayan sayısal değer,Tamsayı değeri,Dize değeri veya Boolean değeri<br/> sorgu parametresi olarak kullanmak için. Yalnızca parameterType değer olduğunda kullanılır.|



###  Ayrıca bakınız
* modül [aspose.cells.externalconnections](..)
