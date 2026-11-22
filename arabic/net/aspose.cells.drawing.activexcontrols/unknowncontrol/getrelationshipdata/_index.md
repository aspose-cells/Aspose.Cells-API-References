---
title: "UnknownControl.GetRelationshipData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة UnknownControl. تحصل على البيانات المرتبطة"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/unknowncontrol/getrelationshipdata/
---
## UnknownControl.GetRelationshipData method

يحصل على البيانات المرتبطة.

```csharp
public byte[] GetRelationshipData(string relId)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| relId | String | معرّف العلاقة. |

### قيمة الإرجاع

يرجع البيانات المرتبطة.

### أمثلة

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

            // محاولة إضافة عنصر تحكم ActiveX غير معروف
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

            // احصل على العنصر كـ UnknownControl
            UnknownControl unknownControl = shape.ActiveXControl as UnknownControl;
            if (unknownControl == null)
            {
                Console.WriteLine("ActiveX control is not UnknownControl type");
                return;
            }

            try
            {
                // تنفيذ GetRelationshipData مع معامل نصي
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

### انظر أيضًا

* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


