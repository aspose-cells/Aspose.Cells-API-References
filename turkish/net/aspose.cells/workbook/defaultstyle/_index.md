---
title: DefaultStyle
second_title: Aspose.Cells for .NET API Referansı
description: Varsayılanı alır veya ayarlarStyleaspose.cells/style çalışma kitabının nesnesi.
type: docs
weight: 130
url: /tr/net/aspose.cells/workbook/defaultstyle/
---
## Workbook.DefaultStyle property

Varsayılanı alır veya ayarlar[`Style`](../../style) çalışma kitabının nesnesi.

```csharp
public Style DefaultStyle { get; set; }
```

### Notlar

DefaultStyle özelliği, tüm Çalışma Kitabı için bir Stil uygulamak için kullanışlıdır.

### Örnekler

Aşağıdaki kod, yeni bir Çalışma Kitabı oluşturur ve somutlaştırır ve bir varsayılan ayarlar[`Style`](../../style) ona.

```csharp
[C#]
Workbook workbook = new Workbook();
Style defaultStyle = workbook.DefaultStyle;
defaultStyle.Font.Name = "Tahoma";
workbook.DefaultStyle = defaultStyle;

[Visual Basic]
Dim workbook as Workbook = new Workbook()
Dim defaultStyle as Style = workbook.DefaultStyle
defaultStyle.Font.Name = "Tahoma"
workbook.DefaultStyle = defaultStyle
```

### Ayrıca bakınız

* class [Style](../../style)
* class [Workbook](../../workbook)
* ad alanı [Aspose.Cells](../../workbook)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
