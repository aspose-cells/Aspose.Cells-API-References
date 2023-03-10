---
title: DBConnection sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 30
url: /tr/python-net/aspose.cells.externalconnections/dbconnection/
is_root: false
---
##  DBConnection sınıfı
Bir ODBC veya OLE DB dış veri bağlantısıyla ilişkili tüm özellikleri belirtir.



**Miras:** [DBConnection](/cells/python-net/aspose.cells.externalconnections/dbconnection) → 
[ExternalConnection](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection)



DBConnection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [id](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/id) | Bağlantının kimliğini alır.|
| [power_query_formula](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/power_query_formula) | Güçlü sorgu formülünün tanımını alır.|
| [type](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/type) | Dış bağlantı DataSource türünü alır veya ayarlar.|
| [source_file](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/source_file) | Harici veri kaynağı dosya tabanlı olduğunda kullanılır. Böyle bir veriye bağlantı kurulduğunda<br/> kaynak başarısız olursa, elektronik tablo uygulaması doğrudan bu dosyaya bağlanmaya çalışır. Belki<br/> URI veya sisteme özel dosya yolu notasyonu ile ifade edilir.|
| [sso_id](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/sso_id) | Bir aracı arasında kimlik doğrulama için kullanılan Çoklu Oturum Açma (SSO) tanımlayıcısı<br/> elektronik tabloML sunucusu ve harici veri kaynağı.|
| [save_password](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/save_password) | Parola bağlantı dizesinin bir parçası olarak kaydedilecekse doğrudur; Aksi takdirde, Yanlış.|
| [save_data](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/save_data) | Bir tabloyu doldurmak için bağlantı üzerinden getirilen harici veriler kaydedilecekse doğrudur.<br/> çalışma kitabı ile; Aksi takdirde, yanlış.|
| [refresh_on_load](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/refresh_on_load) | Dosya açılırken bu bağlantının yenilenmesi gerekiyorsa doğrudur; Aksi takdirde, yanlış.|
| [reconnection_method_type](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method_type) | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir.<br/>Varsayılan değer ReConnectionMethodType.Required şeklindedir.|
| [reconnection_method](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method) | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir.<br/>Varsayılan değer ReConnectionMethodType.Required şeklindedir.|
| [only_use_connection_file](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/only_use_connection_file) | Elektronik tablo uygulamasının her zaman ve yalnızca<br/> odcFile özniteliği tarafından belirtilen harici bağlantı dosyasındaki bağlantı bilgileri<br/> bağlantı yenilendiğinde. Yanlışsa, elektronik tablo uygulaması<br/> reconnectionMethod özniteliği tarafından belirtilen prosedürü izlemelidir|
| [odc_file](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/odc_file) | Bu bağlantının yapıldığı harici bağlantı dosyasının tam yolunu belirtir.<br/> oluşturuldu. Verileri yenileme girişimi sırasında bir bağlantı başarısız olursa ve reconnectionMethod=1,<br/> ardından elektronik tablo uygulaması, harici bağlantı dosyasındaki bilgileri kullanarak tekrar deneyecektir.<br/> çalışma kitabına katıştırılmış bağlantı nesnesi yerine.|
| [is_new](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/is_new) | Bağlantı ilk kez yenilenmediyse doğrudur; Aksi takdirde, yanlış.<br/> Bu durum, bir sorgunun döndürülmesi tamamlanmadan önce kullanıcı dosyayı kaydettiğinde gerçekleşebilir.|
| [name](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/name) | Bağlantının adını belirtir. Her bağlantının benzersiz bir adı olmalıdır.|
| [keep_alive](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/keep_alive) | Elektronik tablo uygulamasının bağlantıyı sürdürmek için çaba göstermesi gerektiğinde doğrudur<br/>açık. Yanlış olduğunda, uygulama, bağlantıyı aldıktan sonra bağlantıyı kapatmalıdır.<br/> bilgi.|
| [refresh_internal](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/refresh_internal) | Bağlantının otomatik yenilemeleri arasındaki dakika sayısını belirtir.|
| [connection_id](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/connection_id) | Bu bağlantının benzersiz tanımlayıcısını belirtir.|
| [connection_description](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/connection_description) | Bu bağlantı için kullanıcı açıklamasını belirtir|
| [is_deleted](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/is_deleted) |İlişkili çalışma kitabı bağlantısının silinip silinmediğini gösterir. doğru ise<br/> bağlantı silindi; Aksi takdirde, yanlış.|
| [credentials_method_type](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/credentials_method_type) | Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir.|
| [credentials](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/credentials) | Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir.|
| [background_refresh](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/background_refresh) | Bağlantının arka planda (eşzamansız olarak) yenilenip yenilenemeyeceğini belirtir.<br/>true bağlantının tercih edilen kullanımı arka planda eşzamansız olarak yenilemekse;<br/> false bağlantının tercih edilen kullanımı ön planda eşzamanlı olarak yenilemekse.|
| [parameters](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/parameters) | ODBC veya web sorgusu için [ConnectionParameterCollection](/cells/tr/python-net/aspose.cells.externalconnections/connectionparametercollection) alır.|
| [connection_info](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/connection_info) | Bağlantı bilgisi dizesi, bir OLE DB veya ODBC veri kaynağıyla bağlantı kurmak için kullanılır.|
| [command_type](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/command_type) | OLE DB komut türünü belirtir.<br/>1. Sorgu bir küp adını belirtir<br/>2. Sorgu, bir SQL deyimi belirtir<br/>3. Sorgu bir tablo adı belirtir<br/>4. Sorgu, varsayılan bilginin verildiğini belirtir ve nasıl yorumlanacağı sağlayıcıya bağlıdır.<br/> 5. Sorgu, web tabanlı bir Liste Veri Sağlayıcıya yöneliktir.|
| [command](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/command) | API veri sağlayıcısına iletilecek veritabanı komutunu içeren dize<br/> veri almak için dış kaynakla etkileşim|
| [sever_command](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection/sever_command) |PivotTable sunucu tabanlı olduğunda kalıcı olan ikinci bir komut metni dizesi belirtir.<br/> sayfa alanları kullanımda.<br/> ODBC bağlantıları için, serverCommand genellikle komuttan daha geniş bir sorgudur (no<br/>WHERE yan tümcesi öncekinde bulunur). Bu 2 komuta (Command ve ServerCommand) dayalı olarak,<br/> parametre kullanıcı arabirimi doldurulabilir ve parametreleştirilmiş sorgular oluşturulabilir|



###  Ayrıca bakınız
* modül [aspose.cells.externalconnections](..)
* sınıf [ConnectionParameterCollection](/cells/tr/python-net/aspose.cells.externalconnections/connectionparametercollection)
* sınıf [DBConnection](/cells/tr/python-net/aspose.cells.externalconnections/dbconnection)
* sınıf [ExternalConnection](/cells/tr/python-net/aspose.cells.externalconnections/externalconnection)
