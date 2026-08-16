---
title: Aspose::Cells::Drawing::FillFormat class
linktitle: FillFormat
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::FillFormat class. Encapsulates the object that represents fill formatting for a shape in C++.'
type: docs
weight: 1700
url: /it/cpp/aspose.cells.drawing/fillformat/
---
## FillFormat class


Encapsulates the object that represents fill formatting for a shape.

```cpp
class FillFormat
```

## Methods

| Method | Description |
| --- | --- |
| [Equals(const Aspose::Cells::Object\& obj)](./equals/) |  |
| [FillFormat(FillFormat_Impl* impl)](./fillformat/) | Constructs from an implementation object. |
| [FillFormat(const FillFormat\& src)](./fillformat/) | Copy constructor. |
| [GetFillType()](./getfilltype/) | Gets and sets fill type. |
| [GetGradientColor1()](./getgradientcolor1/) | Returns the gradient color 1 for the specified fill. |
| [GetGradientColor2()](./getgradientcolor2/) | Returns the gradient color 2 for the specified fill. |
| [GetGradientColorType()](./getgradientcolortype/) | Returns the gradient color type for the specified fill. |
| [GetGradientDegree()](./getgradientdegree/) | Returns the gradient degree for the specified fill. Only applies for Excel 2007. |
| [GetGradientFill()](./getgradientfill/) | Gets [GradientFill](../gradientfill/) object. |
| [GetGradientStyle()](./getgradientstyle/) | Returns the gradient style for the specified fill. |
| [GetGradientVariant()](./getgradientvariant/) | Returns the gradient variant for the specified fill. Only applies for Excel 2007. |
| [GetHashCode()](./gethashcode/) | Gets the hash code. |
| [GetImageData()](./getimagedata/) | Gets and sets the picture image data. |
| [GetPattern()](./getpattern/) | Represents an area's display pattern. |
| [GetPatternFill()](./getpatternfill/) | Gets [PatternFill](../patternfill/) object. |
| [GetPictureFormatType()](./getpictureformattype/) | Gets and sets the picture format type. |
| [GetPresetColor()](./getpresetcolor/) | Returns the gradient preset color for the specified fill. |
| [GetScale()](./getscale/) | Gets and sets the picture format scale. |
| [GetSolidFill()](./getsolidfill/) | Gets [SolidFill](../solidfill/) object. |
| [GetTexture()](./gettexture/) | Represents the texture type for the specified fill. |
| [GetTextureFill()](./gettexturefill/) | Gets [TextureFill](../texturefill/) object. |
| [GetTransparency()](./gettransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const FillFormat\& src)](./operator_asm/) | operator= |
| [SetFillType(FillType value)](./setfilltype/) | Gets and sets fill type. |
| [SetImageData(const Vector \<uint8_t\>\& value)](./setimagedata/) | Gets and sets the picture image data. |
| [SetOneColorGradient(const Aspose::Cells::Color\& color, double degree, GradientStyleType style, int32_t variant)](./setonecolorgradient/) | Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [SetPattern(FillPattern value)](./setpattern/) | Represents an area's display pattern. |
| [SetPictureFormatType(FillPictureType value)](./setpictureformattype/) | Gets and sets the picture format type. |
| [SetPresetColorGradient(GradientPresetType presetColor, GradientStyleType style, int32_t variant)](./setpresetcolorgradient/) | Sets the specified fill to a preset-color gradient. Only applies for Excel 2007. |
| [SetScale(double value)](./setscale/) | Gets and sets the picture format scale. |
| [SetTexture(TextureType value)](./settexture/) | Represents the texture type for the specified fill. |
| [SetTransparency(double value)](./settransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [SetTwoColorGradient(const Aspose::Cells::Color\& color1, const Aspose::Cells::Color\& color2, GradientStyleType style, int32_t variant)](./settwocolorgradient/) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [SetTwoColorGradient(const Aspose::Cells::Color\& color1, double transparency1, const Aspose::Cells::Color\& color2, double transparency2, GradientStyleType style, int32_t variant)](./settwocolorgradient/) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [~FillFormat()](./~fillformat/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Istanziare un oggetto Workbook
Workbook workbook;
//Aggiungere un nuovo foglio di lavoro all'oggetto Excel
int sheetIndex = workbook.GetWorksheets().Add();
//Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Aggiunta di un valore di esempio alla cella "A1"
worksheet.GetCells().Get(u"A1").PutValue(50);
//Aggiunta di un valore di esempio alla cella "A2"
worksheet.GetCells().Get(u"A2").PutValue(100);
//Aggiunta di un valore di esempio alla cella "A3"
worksheet.GetCells().Get(u"A3").PutValue(150);
//Aggiunta di un valore di esempio alla cella "A4"
worksheet.GetCells().Get(u"A4").PutValue(200);
//Aggiunta di un valore di esempio alla cella "B1"
worksheet.GetCells().Get(u"B1").PutValue(60);
//Aggiunta di un valore di esempio alla cella "B2"
worksheet.GetCells().Get(u"B2").PutValue(32);
//Aggiunta di un valore di esempio alla cella "B3"
worksheet.GetCells().Get(u"B3").PutValue(50);
//Aggiunta di un valore di esempio alla cella "B4"
worksheet.GetCells().Get(u"B4").PutValue(40);
//Aggiunta di un valore di esempio alla cella "C1" come dati di categoria
worksheet.GetCells().Get(u"C1").PutValue(u"Q1");
//Aggiunta di un valore di esempio alla cella "C2" come dati di categoria
worksheet.GetCells().Get(u"C2").PutValue(u"Q2");
//Aggiunta di un valore di esempio alla cella "C3" come dati di categoria
worksheet.GetCells().Get(u"C3").PutValue(u"Y1");
//Aggiunta di un valore di esempio alla cella "C4" come dati di categoria
worksheet.GetCells().Get(u"C4").PutValue(u"Y2");
//Aggiunta di un grafico al foglio di lavoro
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Accesso all'istanza del grafico appena aggiunto
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Aggiunta di NSeries (origine dati del grafico) al grafico che va dalla cella "A1" alla "B4"
int seriesIndex = chart.GetNSeries().Add(u"A1:B4", true);
//Impostazione dell'origine dati per i dati di categoria di NSeries
chart.GetNSeries().SetCategoryData(u"C1:C4");
//Riempire l'area della seconda NSeries con una sfumatura
chart.GetNSeries().Get(seriesIndex).GetArea().GetFillFormat().SetOneColorGradient(Color{ 0xff,0,0xff,0 }, 1, GradientStyleType::Horizontal, 1);

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
