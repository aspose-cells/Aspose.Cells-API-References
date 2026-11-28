---
title: "GradientStopCollection sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.GradientStopCollection sınıfı. Gradyan durak koleksiyonunu temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/gradientstopcollection/
---
## GradientStopCollection class

Gradyan durak noktası koleksiyonunu temsil eder.

```csharp
public class GradientStopCollection : CollectionBase<GradientStop>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/gradientstopcollection/item/) { get; } | İndeks ile gradyan durakını alır. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.drawing/gradientstopcollection/add/#add)(double, CellsColor, int) | Bir gradyan durak ekleyin. |
| [Add](../../aspose.cells.drawing/gradientstopcollection/add/#add_1)(double, Color, int) | Bir gradyan durak ekleyin. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(GradientStop) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(GradientStop, IComparer&lt;GradientStop&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, GradientStop, IComparer&lt;GradientStop&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(GradientStop) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(GradientStop[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(GradientStop[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, GradientStop[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;GradientStop&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;GradientStop&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;GradientStop&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;GradientStop&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;GradientStop&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;GradientStop&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;GradientStop&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;GradientStop&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;GradientStop&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;GradientStop&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(GradientStop) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(GradientStop, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(GradientStop, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(GradientStop) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(GradientStop, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(GradientStop, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassGradientStopCollectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Gradyan dolgu ile bir dikdörtgen şekil oluşturun
                var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 300, 100);
                shape.Fill.FillType = FillType.Gradient;

                // Şeklin gradyan dolgusundan GradientStopCollection'ı alın
                GradientStopCollection gradientStops = shape.Fill.GradientFill.GradientStops;
                gradientStops.Clear();

                // Mevcut iki Add yöntemiyle gradyan durakları ekleyin
                gradientStops.Add(0.0, Color.Red, 255); // Opaque red at start
                gradientStops.Add(0.5, Color.Yellow, 200); // Semi-transparent yellow at middle

                // Bir CellsColor oluşturun ve başka bir gradyan durak ekleyin
                CellsColor customColor = workbook.CreateCellsColor();
                customColor.Color = Color.Blue;
                gradientStops.Add(1.0, customColor, 150); // Semi-transparent blue at end

                Console.WriteLine("GradientStopCollection created and populated successfully");
                workbook.Save("GradientStopCollectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientStopCollection: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [GradientStop](../gradientstop/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


