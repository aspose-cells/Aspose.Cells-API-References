---
title: "WorkbookSettings.DefaultStyleSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings property. Bu çalışma kitabı için stil ile ilgili özelliklerin varsayılan değer ayarlarını alır"
type: docs
url: /tr/net/aspose.cells/workbooksettings/defaultstylesettings/
---
## WorkbookSettings.DefaultStyleSettings property

Bu çalışma kitabı için stil ile ilgili özelliklerin varsayılan değer ayarlarını alır.

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Örnekler

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Varsayılan stil ayarlarına eriş
            DefaultStyleSettings styleSettings = workbook.Settings.DefaultStyleSettings;

            // Yerleşik sayı biçimi tercihini ayarla
            styleSettings.BuiltInPreference = true;

            // Sayı biçimlendirme için kültürü ayarla
            workbook.Settings.CultureInfo = new CultureInfo("en-US");

            // Hücrelere eriş ve biçimlendirme uygula
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Değerleri ve stilleri ayarlayın
            cells["A1"].PutValue(1234.56);
            cells["A1"].GetStyle().Number = 4; // Currency format

            cells["B1"].PutValue(0.456);
            cells["B1"].GetStyle().Number = 2; // Percentage format

            cells["C1"].PutValue(DateTime.Now);
            cells["C1"].GetStyle().Number = 22; // Short date format

            // Çalışma kitabını kaydedin
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


