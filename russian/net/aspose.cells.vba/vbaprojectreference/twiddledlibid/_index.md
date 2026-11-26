---
title: "VbaProjectReference.Twiddledlibid"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProjectReference. Получает и задает изменённый Libid ссылки"
type: docs
url: /ru/net/aspose.cells.vba/vbaprojectreference/twiddledlibid/
---
## VbaProjectReference.Twiddledlibid property

Получает и задает изменённый (twiddled) Libid ссылки.

```csharp
public string Twiddledlibid { get; set; }
```

### Примечания

Только для ссылки на элемент управления.

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyTwiddledlibidDemo
    {
        public static void Run()
        {
            Workbook sourceWorkbook = new Workbook("source.xlsm");
            Workbook targetWorkbook = new Workbook();
            
            targetWorkbook.VbaProject.References.Clear();
            
            foreach (VbaProjectReference refSrc in sourceWorkbook.VbaProject.References)
            {
                if (refSrc.Type == VbaProjectReferenceType.Control)
                {
                    targetWorkbook.VbaProject.References.AddControlRefrernce(
                        refSrc.Name,
                        refSrc.Libid,
                        refSrc.Twiddledlibid,
                        refSrc.ExtendedLibid);
                }
            }
            
            targetWorkbook.Save("output.xlsm");
        }
    }
}
```

### См. также

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


