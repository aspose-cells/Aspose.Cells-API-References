---
title: AbstractCalculationEngine sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells/abstractcalculationengine/
is_root: false
---
##  AbstractCalculationEngine sınıfı
Aspose.Cells varsayılan hesaplama motorunu genişletmek için kullanıcının özel hesaplama motorunu temsil eder.



AbstractCalculationEngine türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [is_param_literal_required](/cells/tr/python-net/aspose.cells/abstractcalculationengine/is_param_literal_required) | Hesaplama yaparken bu motorun parametrenin değişmez metnine ihtiyaç duyup duymadığını gösterir. Varsayılan değer yanlıştır.|
| [process_built_in_functions](/cells/tr/python-net/aspose.cells/abstractcalculationengine/process_built_in_functions) | Yerleşik motor tarafından desteklenen yerleşik işlevlerin bu uygulama tarafından kontrol edilip işlenmesi gerekip gerekmediği.<br/>Varsayılan yanlıştır.<br/> Kullanıcının bazı yerleşik fonksiyonların hesaplama mantığını değiştirmesi gerekiyorsa, bu özellik true olarak ayarlanmalıdır.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [calculate(data)](/cells/tr/python-net/aspose.cells/abstractcalculationengine/calculate/#CalculationData) | Verilen verilerle bir işlevi hesaplar.|



###  Notlar

Kullanıcı, bu uygulamada Çalışma Kitabının herhangi bir bölümünü doğrudan değiştirmemelidir (CalculationData.CalculatedValue özelliği tarafından ayarlanabilen özel işlevin hesaplanan sonucu dışında).
Aksi takdirde beklenmeyen sonuç veya İstisna meydana gelebilir.
Kullanıcının, bazı özel işlevler için uygulamada hesaplanan sonuçlar dışındaki verileri değiştirmesi gerekiyorsa,
örneğin, hücrenin formülünü, stilini vb. değiştirmek, kullanıcı bu verileri bu uygulamada toplamalı ve formül hesaplama kapsamı dışında değiştirmelidir.

###  Ayrıca bakınız
* modül [aspose.cells](..)
