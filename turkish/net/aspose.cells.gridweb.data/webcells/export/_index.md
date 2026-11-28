---
title: "WebCells.Export"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebCells yöntemi. Bir WebWorksheet'in Cells koleksiyonundaki verileri yeni bir DataTable nesnesine dışa aktarır."
type: docs
url: /tr/net/aspose.cells.gridweb.data/webcells/export/
---
## WebCells.Export method

Bir WebWorksheet'in Cells koleksiyonundaki verileri yeni bir DataTable nesnesine dışa aktarır.

```csharp
public DataTable Export(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Dışa aktarılacak ilk hücrenin satır numarası. |
| startColumn | Int32 | Dışa aktarılacak ilk hücrenin sütun numarası. |
| satırlar | Int32 | İçe aktarılacak satır sayısı. |
| sütunlar | Int32 | İçe aktarılacak sütun sayısı. |
| exportColumnName | Boolean | İlk satırdaki verilerin DataTable'ın sütun adı olarak dışa aktarılıp aktarılmadığını gösterir |
| isVertical | Boolean | Excel dosyasındaki bir satır DataTable'da bir satırı temsil ediyorsa True. Excel dosyasındaki bir sütun DataTable'da bir satırı temsil ediyorsa False. |

### Dönüş Değeri

Dışa aktarılmış DataTable nesnesi.

### Ayrıca Bakınız

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


