---
title: Font sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 650
url: /tr/python-net/aspose.cells/font/
is_root: false
---
##  Font sınıfı
Elektronik tabloda kullanılan yazı tipi nesnesini kapsüller.



Font türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [charset](/cells/tr/python-net/aspose.cells/font/charset) | Karakter kümesini temsil eder.|
| [is_italic](/cells/tr/python-net/aspose.cells/font/is_italic) | Yazı tipinin italik olup olmadığını gösteren bir değer alır veya ayarlar.|
| [is_bold](/cells/tr/python-net/aspose.cells/font/is_bold) |Yazı tipinin kalın olup olmadığını gösteren bir değer alır veya ayarlar.|
| [caps_type](/cells/tr/python-net/aspose.cells/font/caps_type) | Metin büyük harf türünü alır ve ayarlar.|
| [strike_type](/cells/tr/python-net/aspose.cells/font/strike_type) | Metnin vuruş tipini alır.|
| [is_strikeout](/cells/tr/python-net/aspose.cells/font/is_strikeout) | Yazı tipinin tek çizili olup olmadığını gösteren bir değer alır veya ayarlar.|
| [script_offset](/cells/tr/python-net/aspose.cells/font/script_offset) | Komut dosyası ofsetini yüzde birimi cinsinden alır ve ayarlar|
| [is_superscript](/cells/tr/python-net/aspose.cells/font/is_superscript) | Yazı tipinin süper betik olup olmadığını gösteren bir değer alır veya ayarlar.|
| [is_subscript](/cells/tr/python-net/aspose.cells/font/is_subscript) | Yazı tipinin alt simge olup olmadığını gösteren bir değer alır veya ayarlar.|
| [underline](/cells/tr/python-net/aspose.cells/font/underline) | Yazı tipi altı çizili türünü alır veya ayarlar.|
| [name](/cells/tr/python-net/aspose.cells/font/name) | [Font](/cells/tr/python-net/aspose.cells/font)'in adını alır veya ayarlar.|
| [double_size](/cells/tr/python-net/aspose.cells/font/double_size) | Yazı tipinin çift boyutunu alır ve ayarlar.|
| [size](/cells/tr/python-net/aspose.cells/font/size) | Yazı tipinin boyutunu alır veya ayarlar.|
| [theme_color](/cells/tr/python-net/aspose.cells/font/theme_color) | Tema rengini alır ve ayarlar.|
| [color](/cells/tr/python-net/aspose.cells/font/color) | Yazı tipinin Rengini alır veya ayarlar.|
| [argb_color](/cells/tr/python-net/aspose.cells/font/argb_color) | Rengi 32 bit ARGB değeriyle alır ve ayarlar.|
| [is_normalize_heights](/cells/tr/python-net/aspose.cells/font/is_normalize_heights) | Metne uygulanacak olan yüksekliğin normalizasyonunun normalize edilip edilmediğini gösterir.|
| [scheme_type](/cells/tr/python-net/aspose.cells/font/scheme_type) | Yazı tipinin şema türünü alır ve ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [equals(font)](/cells/tr/python-net/aspose.cells/font/equals/#Font) | İki yazı tipinin eşit olup olmadığını kontrol eder.|



###  örnekler

```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Accessing the "A1" cell from the worksheet
cell = worksheet.cells.get("A1")
# Adding some value to the "A1" cell
cell.put_value("Hello Aspose!")
font = cell.get_style().font
# Setting the font name to "Times New Roman"
font.name = "Times New Roman"
# Setting font size to 14
font.size = 14
# setting font color as Red
font.color = Color.red
# Saving the Excel file
workbook.save(r"dest.xls")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [Font](/cells/tr/python-net/aspose.cells/font)
