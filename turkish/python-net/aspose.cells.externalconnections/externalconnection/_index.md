---
title: ExternalConnection sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 50
url: /tr/python-net/aspose.cells.externalconnections/externalconnection/
is_root: false
---
##  ExternalConnection sınıfı
Harici bir veri bağlantısını belirtir



ExternalConnection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [id](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/id) | Bağlantının kimliğini alır.|
| [power_query_formula](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/power_query_formula) | Güçlü sorgu formülünün tanımını alır.|
| [type](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/type) | Dış bağlantı DataSource türünü alır veya ayarlar.|
| [source_file](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/source_file) | Harici veri kaynağı dosya tabanlı olduğunda kullanılır.<br/> kaynak başarısız olursa, elektronik tablo uygulaması doğrudan bu dosyaya bağlanmaya çalışır.<br/> URI veya sisteme özel dosya yolu notasyonu ile ifade edilir.|
| [sso_id](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/sso_id) | Bir aracı arasında kimlik doğrulama için kullanılan Çoklu Oturum Açma (SSO) tanımlayıcısı<br/> elektronik tabloML sunucusu ve harici veri kaynağı.|
| [save_password](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/save_password) | Parola bağlantı dizesinin bir parçası olarak kaydedilecekse true, aksi takdirde False.|
| [save_data](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/save_data) | Bir tabloyu doldurmak için bağlantı üzerinden getirilen harici veriler kaydedilecekse doğrudur.<br/> çalışma kitabı ile; Aksi takdirde, yanlış.|
| [refresh_on_load](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/refresh_on_load) | Dosya açılırken bu bağlantının yenilenmesi gerekiyorsa doğrudur;|
| [reconnection_method_type](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/reconnection_method_type) | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir.<br/>Varsayılan değer ReConnectionMethodType.Required şeklindedir.|
| [reconnection_method](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/reconnection_method) | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir.<br/>Varsayılan değer ReConnectionMethodType.Required şeklindedir.|
| [only_use_connection_file](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/only_use_connection_file) | Elektronik tablo uygulamasının her zaman ve yalnızca<br/> odcFile özniteliği tarafından belirtilen harici bağlantı dosyasındaki bağlantı bilgileri<br/> bağlantı yenilendiğinde. Yanlışsa elektronik tablo uygulaması<br/> reconnectionMethod özniteliği tarafından belirtilen prosedürü izlemelidir|
| [odc_file](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/odc_file) | Bu bağlantının yapıldığı harici bağlantı dosyasının tam yolunu belirtir.<br/> Verileri yenileme girişimi sırasında bir bağlantı başarısız olursa ve reconnectionMethod=1,<br/> ardından elektronik tablo uygulaması, harici bağlantı dosyasındaki bilgileri kullanarak tekrar deneyecektir.<br/> çalışma kitabına katıştırılmış bağlantı nesnesi yerine.|
| [is_new](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/is_new) | Bağlantı ilk kez yenilenmediyse doğru, aksi takdirde yanlış.<br/> Bu durum, bir sorgunun döndürülmesi tamamlanmadan önce kullanıcı dosyayı kaydettiğinde gerçekleşebilir.|
| [name](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/name) | Bağlantının adını belirtir.|
| [keep_alive](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/keep_alive) | Elektronik tablo uygulamasının bağlantıyı sürdürmek için çaba göstermesi gerektiğinde doğrudur<br/>false olduğunda, uygulama bağlantıyı aldıktan sonra bağlantıyı kapatmalıdır.<br/> bilgi.|
| [refresh_internal](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/refresh_internal) | Bağlantının otomatik yenilemeleri arasındaki dakika sayısını belirtir.|
| [connection_id](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/connection_id) | Bu bağlantının benzersiz tanımlayıcısını belirtir.|
| [connection_description](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/connection_description) | Bu bağlantı için kullanıcı açıklamasını belirtir|
| [is_deleted](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/is_deleted) |İlişkili çalışma kitabı bağlantısının silinip silinmediğini gösterir.<br/> Aksi takdirde, yanlış.|
| [credentials_method_type](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/credentials_method_type) | Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir.|
| [credentials](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/credentials) | Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir.|
| [background_refresh](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/background_refresh) | Bağlantının arka planda (eşzamansız olarak) yenilenip yenilenemeyeceğini belirtir.<br/>true bağlantının tercih edilen kullanımı arka planda eşzamansız olarak yenilemekse;<br/> false bağlantının tercih edilen kullanımı ön planda eşzamanlı olarak yenilemekse.|
| [parameters](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection/parameters) | ODBC veya web sorgusu için [ConnectionParameterCollection](/cells/tr/python-net/aspose.cells.externalconnections/connectionparametercollection) alır.|



###  Ayrıca bakınız
* modül [aspose.cells.externalconnections](..)
* sınıf [ConnectionParameterCollection](/cells/tr/python-net/aspose.cells.externalconnections/connectionparametercollection)
