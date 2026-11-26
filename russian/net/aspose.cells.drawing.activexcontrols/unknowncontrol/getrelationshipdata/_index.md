---
title: "UnknownControl.GetRelationshipData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод UnknownControl. Получает связанные данные"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/unknowncontrol/getrelationshipdata/
---
## UnknownControl.GetRelationshipData method

Получает связанные данные.

```csharp
public byte[] GetRelationshipData(string relId)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| relId | String | Идентификатор связи. |

### Возвращаемое значение

Возвращает связанные данные.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class UnknownControlMethodGetRelationshipDataWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Попытка добавить неизвестный ActiveX‑контрол
            Shape shape;
            try
            {
                shape = worksheet.Shapes.AddActiveXControl(ControlType.Unknown, 0, 0, 0, 0, 100, 100);
            }
            catch (ArgumentException ex)
            {
                Console.WriteLine($"Could not create control: {ex.Message}");
                return;
            }

            // Получить контрол как UnknownControl
            UnknownControl unknownControl = shape.ActiveXControl as UnknownControl;
            if (unknownControl == null)
            {
                Console.WriteLine("ActiveX control is not UnknownControl type");
                return;
            }

            try
            {
                // Выполнить GetRelationshipData со строковым параметром
                string relationshipId = "rId1";
                byte[] relationshipData = unknownControl.GetRelationshipData(relationshipId);

                Console.WriteLine("GetRelationshipData executed successfully");
                Console.WriteLine(relationshipData == null 
                    ? "No relationship data found" 
                    : $"Received {relationshipData.Length} bytes of data");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("UnknownControlGetRelationshipDataDemo.xlsx");
        }
    }
}
```

### См. также

* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


