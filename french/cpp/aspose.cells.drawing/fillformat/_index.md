---
title: Aspose::Cells::Drawing::FillFormat class
linktitle: FillFormat
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::FillFormat class. Encapsulates the object that represents fill formatting for a shape in C++.'
type: docs
weight: 1700
url: /fr/cpp/aspose.cells.drawing/fillformat/
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
//Instanciation d'un objet Workbook
Workbook workbook;
//Ajout d'une nouvelle feuille de calcul à l'objet Excel
int sheetIndex = workbook.GetWorksheets().Add();
//Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Ajouter une valeur d'exemple à la cellule \"A1\"
worksheet.GetCells().Get(u"A1").PutValue(50);
//Ajouter une valeur d'exemple à la cellule \"A2\"
worksheet.GetCells().Get(u"A2").PutValue(100);
//Ajouter une valeur d'exemple à la cellule \"A3\"
worksheet.GetCells().Get(u"A3").PutValue(150);
//Ajouter une valeur d'exemple à la cellule \"A4\"
worksheet.GetCells().Get(u"A4").PutValue(200);
//Ajouter une valeur d'exemple à la cellule \"B1\"
worksheet.GetCells().Get(u"B1").PutValue(60);
//Ajouter une valeur d'exemple à la cellule \"B2\"
worksheet.GetCells().Get(u"B2").PutValue(32);
//Ajouter une valeur d'exemple à la cellule \"B3\"
worksheet.GetCells().Get(u"B3").PutValue(50);
//Ajouter une valeur d'exemple à la cellule \"B4\"
worksheet.GetCells().Get(u"B4").PutValue(40);
//Ajouter une valeur d'exemple à la cellule \"C1\" en tant que donnée de catégorie
worksheet.GetCells().Get(u"C1").PutValue(u"Q1");
//Ajouter une valeur d'exemple à la cellule \"C2\" en tant que donnée de catégorie
worksheet.GetCells().Get(u"C2").PutValue(u"Q2");
//Ajouter une valeur d'exemple à la cellule \"C3\" en tant que donnée de catégorie
worksheet.GetCells().Get(u"C3").PutValue(u"Y1");
//Ajouter une valeur d'exemple à la cellule \"C4\" en tant que donnée de catégorie
worksheet.GetCells().Get(u"C4").PutValue(u"Y2");
//Ajouter un graphique à la feuille de calcul
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Accéder à l'instance du graphique nouvellement ajouté
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Ajouter NSeries (source de données du graphique) au graphique allant de la cellule \"A1\" à \"B4\"
int seriesIndex = chart.GetNSeries().Add(u"A1:B4", true);
//Définir la source de données pour les données de catégorie de NSeries
chart.GetNSeries().SetCategoryData(u"C1:C4");
//Remplir la zone de la 2ᵉ NSeries avec un dégradé
chart.GetNSeries().Get(seriesIndex).GetArea().GetFillFormat().SetOneColorGradient(Color{ 0xff,0,0xff,0 }, 1, GradientStyleType::Horizontal, 1);

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
