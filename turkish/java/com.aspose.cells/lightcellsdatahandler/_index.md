---
title: "LightCellsDataHandler"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hafif modda büyük elektronik tablo dosyalarını okumak için hücre veri işleyicisini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/lightcellsdatahandler/
---
```
public interface LightCellsDataHandler
```

Hafif modda büyük elektronik tablo dosyalarını okumak için hücre veri işleyicisini temsil eder.

**Remarks**

Bu modda bir çalışma kitabı okunurken, çalışma kitabındaki her çalışma sayfası okunurken [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) kontrol edilir. Bir sayfa için, eğer [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) true dönerse, bu sayfanın satır/ hücre verileri ve özellikleri bu arayüzün uygulanması tarafından kontrol edilir ve işlenir. Her satır için, [startRow(int)](../../com.aspose.cells/lightcellsdatahandler\#startRow-int-) işlenmesi gerekip gerekmediğini kontrol etmek üzere çağrılır. Bir satır işlenmesi gerekiyorsa, önce bu satırın özellikleri okunur ve kullanıcı bu özelliklere [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-) ile erişebilir. Satırın hücrelerinin de işlenmesi gerekiyorsa, [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-) true döndürmeli ve ardından bu satırdaki mevcut her hücre için [startCell(int)](../../com.aspose.cells/lightcellsdatahandler\#startCell-int-) bir hücrenin işlenip işlenmeyeceğini kontrol etmek üzere çağrılır. Bir hücre işlenmesi gerekiyorsa, [processCell(Cell)](../../com.aspose.cells/lightcellsdatahandler\#processCell-Cell-) bu hücreyi arayüzün uygulanmasıyla işlemek üzere çağrılır.

Lütfen unutmayın, kullanıcı yalnızca ilgili yöntem tarafından sağlanan mevcut Row/Cell nesnesinin değerleri ve özellikleri üzerinde işlem yapmalıdır. Hücre verileri şablon dosyasından akış şeklinde okunduğu için, diğer nesnelerin çoğu hücre verileri yüklendikten sonra yeniden ayarlanabilir/güncellenebilir. Bu nedenle, kullanıcı bu uygulamanın diğer yöntemlerinde başka nesneler üzerinde işlem yaptığında, bu işlemler çalışma kitabındaki mevcut nesneleri etkileyemeyebilir. Daha da kötüsü, bu işlemler çalışma kitabında tutarsız verilere ve sonrasında beklenmeyen sorunlara veya istisnalara yol açabilir. Bu yüzden şekiller, sütun genişlikleri ve stiller, koşullu biçimlendirmeler vb. gibi diğer tüm nesneler bu uygulamanın hiçbir yönteminde işlenmemelidir. Bunun yerine, çalışma kitabı oluşturulduktan sonra bu nesneleri yönetin.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [processCell(Cell cell)](#processCell-com.aspose.cells.Cell-) | Bir hücre işlemeye başlar. |
| [processRow(Row row)](#processRow-com.aspose.cells.Row-) | Bir satır işlemeye başlar. |
| [startCell(int columnIndex)](#startCell-int-) | Bir hücre işlemeye hazırlanır. |
| [startRow(int rowIndex)](#startRow-int-) | Bir satır işlemeye hazırlanır. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | Bir çalışma sayfası işlemeye başlar. |
### processCell(Cell cell) {#processCell-com.aspose.cells.Cell-}
```
public abstract boolean processCell(Cell cell)
```


Bir hücre işlemeye başlar.

**Remarks**

Bir hücrenin verisi okunduktan sonra çağrılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Şu anda işlenen hücre nesnesi |

**Returns:**
boolean - bu hücrenin mevcut sayfanın hücre modeli içinde tutulup tutulmayacağı. Genel olarak false olmalıdır, böylece hücreler işlendiğinde bellekten kaldırılır ve bellek tasarrufu sağlanır. Tüm çalışma kitabı işlendiği halde kullanıcı daha sonra bazı hücrelere erişmek istediği özel durumlarda, bu yöntemin true döndürülmesiyle bu özel hücreler Cells modelinde tutulabilir ve Cells[row, column] gibi API'lerle daha sonra erişilebilir. Ancak, hücre verilerini Cells modelinde tutmak daha fazla bellek gerektirir ve tüm hücreler tutulursa LightCells modunda şablon dosyasının okunması normal şekilde okunmasıyla aynı olur.
### processRow(Row row) {#processRow-com.aspose.cells.Row-}
```
public abstract boolean processRow(Row row)
```


Bir satır işlemeye başlar.

**Remarks**

Satırın yüksekliği, stili vb. özellikleri okunduktan sonra çağrılacaktır. Ancak, bu satırdaki hücreler henüz okunmamıştır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | Şu anda işlenen satır nesnesi. |

**Returns:**
boolean - bu satırın hücrelerinin işlenip işlenmeyeceği. false ise bu satırdaki tüm hücreler yok sayılır.
### startCell(int columnIndex) {#startCell-int-}
```
public abstract boolean startCell(int columnIndex)
```


Bir hücre işlemeye hazırlanır.

**Remarks**

Mevcut satırda mevcut bir hücreye ulaşıldığında çağrılacaktır. Mevcut satır, [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\\#processRow-Row-) metodunun son çağrısının satırıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | işlenecek hücrenin sütun indeksi |

**Returns:**
boolean - bu hücrenin işlenip işlenmeyeceği. false ise hücre yok sayılır ve mevcut satırın hücre verilerinin sonuna ulaşana kadar bir sonraki hücre kontrol edilir
### startRow(int rowIndex) {#startRow-int-}
```
public abstract boolean startRow(int rowIndex)
```


Bir satır işlemeye hazırlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | işlenecek bir sonraki satırın indeksi |

**Returns:**
boolean - bu satırın (özellikleri veya hücre verileri) işlenip işlenmeyeceği. false ise bu satır ve hücreleri yok sayılır ve bir sonraki satır kontrol edilir.
### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public abstract boolean startSheet(Worksheet sheet)
```


Bir çalışma sayfası işlemeye başlar.

**Remarks**

Bir çalışma sayfasının hücre verileri okunmadan önce çağrılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | hücre verileri okunacak çalışma sayfası. |

**Returns:**
boolean - bu sayfanın hücre verilerinin işlenip işlenmeyeceği. false ise bu sayfa yok sayılır.
