---
title: "UnionRange.SetOutlineBorders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод UnionRange. Устанавливает контурные границы вокруг диапазона ячеек"
type: docs
url: /ru/net/aspose.cells/unionrange/setoutlineborders/
---
## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_1}

Устанавливает внешние границы вокруг диапазона ячеек.

```csharp
public void SetOutlineBorders(CellBorderType[] borderStyles, Color[] borderColors)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| borderStyles | CellBorderType[] | Стили границ. |
| borderColors | Color[] | Цвета границ. |

### Примечания

Длина массивов borderStyles и borderStyles должна быть 4. Порядок элементов в borderStyles и borderStyles должен быть верх,низ,лево,право

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetOutlineBordersWithCellBorderTypeAColorArrayDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Test Data");
            worksheet.Cells["A2"].PutValue("More Data");
            worksheet.Cells["B2"].PutValue("Additional Data");

            // Создайте диапазон и преобразуйте его в UnionRange
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");
            UnionRange unionRange = worksheet.Cells.CreateRange(range.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range });

            try
            {
                // Определите стили и цвета границ для всех четырёх сторон
                CellBorderType[] borderStyles = new CellBorderType[]
                {
                    CellBorderType.Thin,    // Top border
                    CellBorderType.Medium,  // Right border
                    CellBorderType.Thick,   // Bottom border
                    CellBorderType.Double   // Left border
                };

                Color[] borderColors = new Color[]
                {
                    Color.Red,     // Top border color
                    Color.Blue,    // Right border color
                    Color.Green,   // Bottom border color
                    Color.Orange   // Left border color
                };

                // Вызовите SetOutlineBorders с массивами
                unionRange.SetOutlineBorders(borderStyles, borderColors);

                Console.WriteLine("SetOutlineBorders method called successfully with CellBorderType[] and Color[] parameters");
                Console.WriteLine($"Applied borders to range: {unionRange.RefersTo}");

                // Сохраните книгу
                workbook.Save("SetOutlineBordersDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOutlineBorders: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [CellBorderType](../../cellbordertype/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders}

Устанавливает контурные границы вокруг диапазона ячеек с одинаковым стилем и цветом границы.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, Color borderColor)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| borderStyle | CellBorderType | Стиль границы. |
| borderColor | Color | Цвет границы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetOutlineBordersWithCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test";
            worksheet.Cells["A2"].Value = "More Data";
            worksheet.Cells["B2"].Value = "Example";

            try
            {
                // Создайте UnionRange, охватывающий A1:B2
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2")
                    .UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

                // Установите контурные границы с определённым типом границы и цветом
                unionRange.SetOutlineBorders(CellBorderType.Medium, Color.Blue);

                Console.WriteLine("SetOutlineBorders method called successfully");
                Console.WriteLine($"Border applied to range: {unionRange.RefersTo}");

                // Сохраните книгу
                workbook.Save("SetOutlineBordersDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOutlineBorders: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [CellBorderType](../../cellbordertype/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


