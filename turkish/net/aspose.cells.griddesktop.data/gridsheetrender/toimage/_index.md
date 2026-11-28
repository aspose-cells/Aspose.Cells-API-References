---
title: "GridSheetRender.ToImage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridSheetRender yöntemi. Belirli bir sayfayı bir Graphics nesnesine render eder"
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridsheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Belirli bir sayfayı Graphics'e render et

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfaIndeksi | Int32 | hangi sayfanın dönüştürüleceğini belirt |
| g | Grafikler | Render yapılacak nesne. |
| x | Single | Render edilen sayfanın sol üst köşesinin X koordinatı (piksel cinsinden). |
| y | Single | Render edilen sayfanın sol üst köşesinin Y koordinatı (piksel cinsinden). |
| genişlik | Single | Render edilen sayfanın kaplayabileceği maksimum genişlik (piksel cinsinden). |
| yükseklik | Single | Render edilen sayfanın kaplayabileceği maksimum yükseklik (piksel cinsinden). |

### Ayrıca Bakınız

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Belirli bir sayfayı Graphics'e render et

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfaIndeksi | Int32 | hangi sayfanın dönüştürüleceğini belirt |
| g | Grafikler | Render yapılacak nesne. |
| x | Single | Render edilen sayfanın sol üst köşesinin X koordinatı (piksel cinsinden). |
| y | Single | Render edilen sayfanın sol üst köşesinin Y koordinatı (piksel cinsinden). |

### Ayrıca Bakınız

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, string) {#toimage_4}

Belirli bir sayfayı bir dosyaya render eder.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfaIndeksi | Int32 | hangi sayfanın dönüştürüleceğini belirt |
| fileName | String | çıktı görüntüsünün dosya adı |

### Örnekler

Aşağıdaki kod, ilk sayfanın ilk sayfasını png görüntüsüne çıkarır.

```csharp
//kaynak dosyayı görüntülerle yükle.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//Çıktı görüntü tipini ayarla.
imgOpt.ImageType = ImageType.Png;

//İlk sayfayı oluştur.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//Sayfanın ilk sayfasını görüntüye çıkar.
sr.ToImage(0, "output.png");
```

### Ayrıca Bakınız

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Stream) {#toimage_3}

Belirli bir sayfayı akıma render eder.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfaIndeksi | Int32 | hangi sayfanın dönüştürüleceğini belirt |
| akış | Stream | çıktı görüntüsünün akışı |

### Ayrıca Bakınız

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int) {#toimage}

Belirli bir sayfayı Bitmap nesnesine render eder.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfaIndeksi | Int32 | hangi sayfanın dönüştürüleceğini belirt |

### Dönüş Değeri

sayfanın bitmap nesnesi

### Ayrıca Bakınız

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


