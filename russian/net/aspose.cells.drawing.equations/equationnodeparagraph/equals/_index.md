---
title: "EquationNodeParagraph.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод EquationNodeParagraph. Определяет, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationnodeparagraph/equals/
---
## EquationNodeParagraph.Equals method

Определить, равен ли текущий узел уравнения указанному узлу

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Object | Указанный узел |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeParagraphMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте два экземпляра EquationNodeParagraph для сравнения
            // Используйте метод CreateNode для правильного создания узлов
            EquationNodeParagraph paragraph1 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
            EquationNodeParagraph paragraph2 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
            
            // Установите разные типы выравнивания, чтобы они стали неравными
            paragraph1.Justification = EquationHorizontalJustificationType.Center;
            paragraph2.Justification = EquationHorizontalJustificationType.Left;

            try
            {
                // Вызовите метод Equals, передав в качестве параметра paragraph2
                bool areEqual = paragraph1.Equals(paragraph2);
                
                // Отобразите результат сравнения
                Console.WriteLine($"Are the paragraphs equal? {areEqual}");

                // Создайте ещё один абзац с тем же выравниванием, что и paragraph1
                EquationNodeParagraph paragraph3 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
                paragraph3.Justification = EquationHorizontalJustificationType.Center;

                // Снова вызовите Equals с paragraph3
                areEqual = paragraph1.Equals(paragraph3);
                Console.WriteLine($"Are paragraph1 and paragraph3 equal? {areEqual}");

                // Также продемонстрируйте сравнение с null
                areEqual = paragraph1.Equals(null);
                Console.WriteLine($"Is paragraph1 equal to null? {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
            
            // Сохраните книгу (хотя видимых изменений в листе не было)
            workbook.Save("EquationNodeParagraphEqualsDemo.xlsx");
        }
    }
}
```

### См. также

* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


