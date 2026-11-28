---
title: "ValidationCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ValidationCollection yöntemi. Koleksiyona bir veri doğrulaması ekler"
type: docs
url: /tr/net/aspose.cells/validationcollection/add/
---
## Add() {#add}

Koleksiyona bir veri doğrulaması ekler.

```csharp
[Obsolete("Use ValidationCollection.Add(CellArea) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add()
```

### Dönüş Değeri

[`Validation`](../../validation/) object index.

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ValidationCollection.Add(CellArea) yöntemini kullanın. Bu yöntem, OCAK 2015'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Ayrıca Bakınız

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(CellArea) {#add_1}

Koleksiyona bir veri doğrulaması ekler.

```csharp
public int Add(CellArea ca)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | CellArea | Alan bu doğrulamayı içerir. |

### Dönüş Değeri

[`Validation`](../../validation/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodAddWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Doğrulama için hücre alanı oluştur
            CellArea cellarea = new CellArea();
            cellarea.StartRow = 0;
            cellarea.StartColumn = 0;
            cellarea.EndRow = 1;
            cellarea.EndColumn = 1;
            
            // Doğrulamayı koleksiyona ekle
            int index = sheet.Validations.Add(cellarea);
            Validation validation = sheet.Validations[index];
            
            // Doğrulama ayarlarını yapılandır
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.AlertStyle = ValidationAlertType.Information;
            
            // Çalışma kitabını kaydedin
            workbook.Save("ValidationCollectionMethodAddWithCellAreaDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


