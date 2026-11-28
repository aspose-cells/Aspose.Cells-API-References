---
title: "Sınıf VbaProjectReference"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Vba.VbaProjectReference sınıfı. VBA projesinin referansını temsil eder"
type: docs
url: /tr/net/aspose.cells.vba/vbaprojectreference/
---
## VbaProjectReference class

VBA projesinin referansını temsil eder.

```csharp
public class VbaProjectReference
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ExtendedLibid](../../aspose.cells.vba/vbaprojectreference/extendedlibid/) { get; set; } | Referansın genişletilmiş Libid değerini alır ve ayarlar. |
| [Libid](../../aspose.cells.vba/vbaprojectreference/libid/) { get; set; } | Referansın Libid değerini alır ve ayarlar. |
| [Name](../../aspose.cells.vba/vbaprojectreference/name/) { get; set; } | Referansın adını alır ve ayarlar. |
| [RelativeLibid](../../aspose.cells.vba/vbaprojectreference/relativelibid/) { get; set; } | Referans verilen VBA projesinin tanımlayıcısını göreceli bir yol ile alır ve ayarlar. |
| [Twiddledlibid](../../aspose.cells.vba/vbaprojectreference/twiddledlibid/) { get; set; } | Referansın twiddled Libid değerini alır ve ayarlar. |
| [Type](../../aspose.cells.vba/vbaprojectreference/type/) { get; } | Bu referansın tipini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaprojectreference/copy/)(VbaProjectReference) |  |

### Örnekler

```csharp

[C#]

//Workbook nesnesi örnekleniyor
Workbook workbook = new Workbook();
 // VBA projesini başlat.
VbaProject vbaProject = workbook.VbaProject;
// VBA proje referansı ekle
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
//Excel dosyasını kaydetme
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Init VBA project.
Dim vbaProject as VbaProject  = workbook.VbaProject
'Add vba project reference
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
'Saving the Excel file
workbook.Save("book1.xlsm")
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


