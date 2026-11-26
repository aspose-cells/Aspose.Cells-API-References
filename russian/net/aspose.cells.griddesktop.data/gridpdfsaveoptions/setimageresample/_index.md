---
title: "GridPdfSaveOptions.SetImageResample"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridPdfSaveOptions. Устанавливает желаемое PPI (pixels per inch) для ресемплинга изображений и качество JPEG. Все изображения будут преобразованы в JPEG с указанным качеством, а изображения, превышающие заданное значение PPI, будут ресемплированы."
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridpdfsaveoptions/setimageresample/
---
## GridPdfSaveOptions.SetImageResample method

Устанавливает желаемое PPI (pixels per inch) для ресемплинга изображений и качество JPEG. Все изображения будут преобразованы в JPEG с указанным параметром качества, и изображения, у которых PPI превышает указанное значение (pixels per inch), будут ресемплированы.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| desiredPPI | Int32 | Желаемое количество пикселей на дюйм. 220 — высокое качество. 150 — качество для экрана. 96 — качество для электронной почты. |
| jpegQuality | Int32 | 0 – 100 % качества JPEG. |

### Примеры

Следующий код устанавливает желаемое значение PPI равным 96 и качество JPEG равным 80 для изображений в выходном PDF.

```csharp
//загрузите исходный файл с изображениями.
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

//установите желаемое значение PPI равным 96 и качество JPEG равным 80.
pdfSaveOptions.SetImageResample(96, 80);

wb.Save("output.pdf", pdfSaveOptions);
```

### См. также

* class [GridPdfSaveOptions](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


