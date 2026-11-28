---
title: "GridJsWorkbook.RedactFile"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridJsWorkbook yöntemi. Bir Excel dosyası üzerinde JSON işlemleri dizisine dayanarak redaksiyon gerçekleştirir."
type: docs
url: /tr/net/aspose.cells.gridjs/gridjsworkbook/redactfile/
---
## GridJsWorkbook.RedactFile method

Excel dosyası üzerinde JSON işlemleri dizisine dayalı redaksiyon gerçekleştirir.

```csharp
public void RedactFile(string excelFilePath, string uid, string[] arrayOfRedactionOpr)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| excelFilePath | String | Redaksiyon yapılacak Excel dosyasının dosya yolu. |
| uid | String | Çalışma kitabı için benzersiz tanımlayıcı. Null veya boş ise, dosya yoluna dayanarak yeni bir uid oluşturulur. |
| arrayOfRedactionOpr | String[] | Uygulanacak redaksiyon işlemlerini temsil eden JSON dizesi dizisi. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| [GridCellException](../../gridcellexception/) | Redaksiyon işlemi sırasında bir CellsException oluştuğunda fırlatılır. |
| Exception | Redaksiyon işlemi sırasında genel bir istisna oluştuğunda fırlatılır. |

### Ayrıca Bakınız

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


