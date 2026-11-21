---
title: "GridCustomServerValidation"
second_title: "Aspose.Cells for Java API Referansı"
description: "Sunucu tarafı doğrulama kullanırken uygulamanız gereken arayüz."
type: docs
url: /tr/java/com.aspose.gridweb/gridcustomservervalidation/
---
```
public interface GridCustomServerValidation
```

sunucu tarafı doğrulama kullanırken uygulamanız gereken arayüz. CustomServerFunction.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [validate(GridWorksheet sheet, int row, int col, String value)](#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-) | **Notlar** |
### validate(GridWorksheet sheet, int row, int col, String value) {#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-}
```
public abstract String validate(GridWorksheet sheet, int row, int col, String value)
```


**Remarks**

eğer string.empty döndürülürse doğrulama geçilir, aksi takdirde ClientCallback işlevinde işlenebilecek ilgili bir mesaj döndürebilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | GridWorksheet |
| satır | int | hücrenin satır indeksi |
| col | int | hücrenin sütun indeksi |
| değer | java.lang.String | doğrulama için değer |

**Returns:**
java.lang.String - dize tabanlı sonuç değeri
