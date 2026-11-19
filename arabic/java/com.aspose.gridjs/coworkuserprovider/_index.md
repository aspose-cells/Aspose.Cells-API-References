---
title: "CoWorkUserProvider"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل واجهة موفر المستخدم في وضع التعاون. متاح الآن فقط في نسخة Java وسيكون متاحًا في نسخة .net/python في المستقبل."
type: docs
url: /ar/java/com.aspose.gridjs/coworkuserprovider/
---
```
public interface CoWorkUserProvider
```

يمثل واجهة موفر المستخدم في وضع التعاون. متاح الآن فقط في نسخة Java، وسيكون متاحًا في نسخة .net/python في المستقبل. يمكن لتطبيق العميل تنفيذ هذه الواجهة لتوفير معلومات المستخدم.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCurrentUserId()](#getCurrentUserId--) | يحصل على المعرف الفريد للمستخدم الحالي |
| [getCurrentUserName()](#getCurrentUserName--) | يحصل على اسم المستخدم للمستخدم الحالي |
| [getPermission()](#getPermission--) | يحصل على مستوى صلاحية المستخدم الحالي |
### getCurrentUserId() {#getCurrentUserId--}
```
public abstract long getCurrentUserId()
```


يحصل على المعرف الفريد للمستخدم الحالي

**Returns:**
long - معرف المستخدم الحالي
### getCurrentUserName() {#getCurrentUserName--}
```
public abstract String getCurrentUserName()
```


يحصل على اسم المستخدم للمستخدم الحالي

**Returns:**
java.lang.String - اسم المستخدم الحالي
### getPermission() {#getPermission--}
```
public abstract int getPermission()
```


يحصل على مستوى صلاحية المستخدم الحالي

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). مستوى صلاحية المستخدم الحالي
