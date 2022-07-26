---
title: Protection
second_title: Aspose.Cells for .NET API Referansı
description: Bir çalışma sayfası için kullanılabilen çeşitli koruma seçenekleri türlerini temsil eder.
type: docs
weight: 4910
url: /tr/net/aspose.cells/protection/
---
## Protection class

Bir çalışma sayfası için kullanılabilen çeşitli koruma seçenekleri türlerini temsil eder.

```csharp
public class Protection
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AllowDeletingColumn](../../aspose.cells/protection/allowdeletingcolumn) { get; set; } | Korumalı bir çalışma sayfasında sütunların silinmesine izin verilip verilmediğini temsil eder. |
| [AllowDeletingRow](../../aspose.cells/protection/allowdeletingrow) { get; set; } | Korumalı bir çalışma sayfasında satırların silinmesine izin verilip verilmediğini temsil eder. |
| [AllowEditingContent](../../aspose.cells/protection/alloweditingcontent) { get; set; } | Kullanıcının korumalı bir çalışma sayfasındaki kilitli hücrelerin içeriğini düzenlemesine izin verilip verilmediğini temsil eder. |
| [AllowEditingObject](../../aspose.cells/protection/alloweditingobject) { get; set; } | Kullanıcının korumalı bir çalışma sayfasındaki çizim nesnelerini değiştirmesine izin verilip verilmediğini temsil eder. |
| [AllowEditingScenario](../../aspose.cells/protection/alloweditingscenario) { get; set; } | Kullanıcının korumalı bir çalışma sayfasındaki senaryoları düzenlemesine izin verilip verilmediğini temsil eder. |
| [AllowFiltering](../../aspose.cells/protection/allowfiltering) { get; set; } | Kullanıcının, sayfa korunmadan önce oluşturulmuş bir Otomatik Filtreyi kullanmasına izin verilip verilmediğini temsil eder. |
| [AllowFormattingCell](../../aspose.cells/protection/allowformattingcell) { get; set; } | Korumalı bir çalışma sayfasında hücrelerin biçimlendirilmesine izin verilip verilmediğini temsil eder. |
| [AllowFormattingColumn](../../aspose.cells/protection/allowformattingcolumn) { get; set; } | Korumalı bir çalışma sayfasında sütunların biçimlendirilmesine izin verilip verilmediğini temsil eder |
| [AllowFormattingRow](../../aspose.cells/protection/allowformattingrow) { get; set; } | Korumalı bir çalışma sayfasında satırların biçimlendirilmesine izin verilip verilmediğini temsil eder |
| [AllowInsertingColumn](../../aspose.cells/protection/allowinsertingcolumn) { get; set; } | Korumalı bir çalışma sayfasında sütun eklenmesine izin verilip verilmediğini temsil eder |
| [AllowInsertingHyperlink](../../aspose.cells/protection/allowinsertinghyperlink) { get; set; } | Korumalı bir çalışma sayfasında köprülerin eklenmesine izin verilip verilmediğini temsil eder |
| [AllowInsertingRow](../../aspose.cells/protection/allowinsertingrow) { get; set; } | Korumalı bir çalışma sayfasında satır eklenmesine izin verilip verilmediğini temsil eder |
| [AllowSelectingLockedCell](../../aspose.cells/protection/allowselectinglockedcell) { get; set; } | Kullanıcının korumalı bir çalışma sayfasında kilitli hücreleri seçmesine izin verilip verilmediğini temsil eder. |
| [AllowSelectingUnlockedCell](../../aspose.cells/protection/allowselectingunlockedcell) { get; set; } | Kullanıcının korumalı bir çalışma sayfasında kilitli olmayan hücreleri seçmesine izin verilip verilmediğini temsil eder. |
| [AllowSorting](../../aspose.cells/protection/allowsorting) { get; set; } | Korumalı bir çalışma sayfasında sıralama seçeneğine izin verilip verilmediğini temsil eder. |
| [AllowUsingPivotTable](../../aspose.cells/protection/allowusingpivottable) { get; set; } | Kullanıcının korumalı bir çalışma sayfasındaki özet tabloları değiştirmesine izin verilip verilmediğini temsil eder. |
| [IsProtectedWithPassword](../../aspose.cells/protection/isprotectedwithpassword) { get; } | Çalışma sayfalarının parola ile korunup korunmadığını gösterir. |
| [Password](../../aspose.cells/protection/password) { get; set; } | Çalışma sayfasını korumak için parolayı temsil eder. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Copy](../../aspose.cells/protection/copy)(Protection) | Koruma bilgilerini kopyalayın. |
| [GetPasswordHash](../../aspose.cells/protection/getpasswordhash)() | Geçerli parolanın karmasını alır. |
| [VerifyPassword](../../aspose.cells/protection/verifypassword)(string) | Şifreyi doğrular. |

### Örnekler

```csharp

[C#]
//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();

Worksheet worksheet = workbook.Worksheets[0];
//Kullanıcıların çalışma sayfasının kilitli hücrelerini seçmesine izin vermek
worksheet.Protection.AllowSelectingLockedCell = true;
//Kullanıcıların çalışma sayfasının kilitli olmayan hücrelerini seçmesine izin verme
worksheet.Protection.AllowSelectingUnlockedCell = true;  

[Visual Basic]

'Bir Çalışma Kitabı nesnesini başlatma
Dim workbook As Workbook = New Workbook()
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Kullanıcıların çalışma sayfasının kilitli hücrelerini seçmesine izin verme
worksheet.Protection.AllowSelectingLockedCell = True
'Kullanıcıların çalışma sayfasının kilitli olmayan hücrelerini seçmesine izin verme
worksheet.Protection.AllowSelectingUnlockedCell = True
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
