# مدير المهام - نظام إدارة المهام والفنيين

نظام شامل لإدارة المهام والفنيين مع ربط بوت التليجرام وإدارة العمولات.

## 🚀 الميزات الرئيسية

### 📊 لوحة التحكم
- إحصائيات شاملة في الوقت الفعلي
- رسوم بيانية تفاعلية
- مؤشرات الأداء الرئيسية
- تتبع الإيرادات من العمولات

### 🔧 إدارة المهام
- إنشاء مهام فردية وجماعية
- تخصيص المهام للفنيين
- تتبع حالة المهام (نشطة، مكتملة، منتهية)
- إرسال المواقع الجغرافية للفنيين
- إدارة التكاليف والعمولات

### 👥 إدارة الفنيين والحرفيين
- قاعدة بيانات شاملة للفنيين
- تتبع التخصصات والمهارات
- إحصائيات الأداء لكل فني
- إدارة الأرباح والمدفوعات

### 🤖 ربط بوت التليجرام
- ربط مباشر مع API التليجرام
- إعداد Webhook للرسائل الفورية
- أوامر تفاعلية للفنيين
- ردود تلقائية ذكية

### 💰 النظام المالي
- إدارة الفواتير والعمولات
- طرق دفع متنوعة (فيزا، تحويل، كاش)
- تتبع التكاليف الفعلية
- تقارير مالية تفصيلية

### 📈 التقارير والتحليلات
- تقارير تفصيلية للفنيين والمهام
- تحليلات الأداء والإيرادات
- تصدير البيانات (CSV, Excel)
- طباعة التقارير

## 🛠️ التقنيات المستخدمة

- **Frontend**: React 18 + TypeScript
- **Styling**: Tailwind CSS
- **Charts**: Recharts
- **Icons**: Lucide React
- **Build Tool**: Vite
- **Date Handling**: date-fns

## 📋 متطلبات النظام

- Node.js 16+ 
- npm أو yarn
- متصفح حديث يدعم ES6+

## 🚀 التثبيت والتشغيل

### 1. تحميل المشروع
```bash
git clone [repository-url]
cd task-manager
```

### 2. تثبيت المكتبات
```bash
npm install
```

### 3. تشغيل النظام محلياً
```bash
npm run dev
```

### 4. بناء النظام للإنتاج
```bash
npm run build
```

## 🌐 النشر على الاستضافة

### نشر على Hostinger (cPanel)

1. **بناء المشروع:**
```bash
npm run build
```

2. **رفع الملفات:**
   - ضغط مجلد `dist` 
   - رفع المحتويات إلى `public_html`
   - التأكد من وجود ملف `.htaccess` للتوجيه

3. **إعداد .htaccess:**
```apache
RewriteEngine On
RewriteCond %{REQUEST_FILENAME} !-f
RewriteCond %{REQUEST_FILENAME} !-d
RewriteRule . /index.html [L]
```

### نشر على الاستضافة السحابية

#### Netlify:
1. ربط المستودع مع Netlify
2. إعداد أوامر البناء:
   - Build command: `npm run build`
   - Publish directory: `dist`

#### Vercel:
1. ربط المستودع مع Vercel
2. النشر التلقائي عند كل تحديث

## 🔧 الإعداد والتكوين

### 1. إعداد بوت التليجرام

1. **إنشاء البوت:**
   - التحدث مع @BotFather في التليجرام
   - استخدام الأمر `/newbot`
   - اختيار اسم ومعرف للبوت
   - نسخ رمز البوت (Bot Token)

2. **ربط البوت بالنظام:**
   - الذهاب إلى تبويب "الإعدادات"
   - إدخال رمز البوت
   - اختبار الاتصال
   - إعداد رابط Webhook

### 2. إعداد Webhook

```
https://your-domain.com/api/webhook
```

### 3. بيانات تسجيل الدخول الافتراضية

- **اسم المستخدم:** `admin`
- **كلمة المرور:** `admin123`

## 📊 خريطة تدفق النظام

```
1. تسجيل الدخول
   ↓
2. لوحة التحكم (عرض الإحصائيات)
   ↓
3. إدارة المهام
   ├── إنشاء مهمة جديدة
   ├── تخصيص للفنيين
   └── تتبع الحالة
   ↓
4. إدارة الفنيين
   ├── عرض قائمة الفنيين
   ├── تتبع الأداء
   └── إدارة الأرباح
   ↓
5. النظام المالي
   ├── إنشا الفواتير
   ├── تسجيل العمولات
   └── طرق الدفع
   ↓
6. التقارير والتحليلات
   ├── تقارير تفصيلية
   ├── تصدير البيانات
   └── طباعة التقارير
```

## 🎯 كيفية الاستخدام

### 1. البداية
- تسجيل الدخول بالبيانات الافتراضية
- مراجعة لوحة التحكم للحصول على نظرة عامة

### 2. إعداد البوت
- الذهاب إلى "الإعدادات"
- إدخال رمز البوت من @BotFather
- اختبار الاتصال وإعداد Webhook

### 3. إدارة الفنيين
- إضافة الفنيين عند تفاعلهم مع البوت لأول مرة
- تحديث معلومات التخصص والمهارات

### 4. إنشاء المهام
- تحديد نوع المهمة (فردية/جماعية)
- إضافة التفاصيل والتكلفة المتوقعة
- تخصيص الفنيين المناسبين
- إضافة الموقع الجغرافي إذا لزم الأمر

### 5. متابعة التنفيذ
- تتبع حالة المهام
- إرسال المواقع للفنيين عند الحاجة
- تحديث حالة المهام حسب التقدم

### 6. إدارة الفواتير
- إنشاء فواتير للمهام المكتملة
- تسجيل التكلفة الفعلية والعمولة
- تحديد طرق الدفع
- متابعة حالة السداد

### 7. التقارير
- مراجعة التقارير التفصيلية
- تصدير البيانات للمراجعة الخارجية
- طباعة التقارير المطلوبة

## 🔒 الأمان

- تشفير كلمات المرور
- حماية API endpoints
- التحقق من صحة البيانات
- حماية من CSRF attacks

## 🆘 الدعم والمساعدة

### المشاكل الشائعة:

1. **فشل اتصال البوت:**
   - التأكد من صحة رمز البوت
   - التحقق من اتصال الإنترنت
   - مراجعة إعدادات Webhook

2. **عدم ظهور البيانات:**
   - تحديث الصفحة
   - مسح cache المتصفح
   - التحقق من console للأخطاء

3. **مشاكل التصدير:**
   - التأكد من دعم المتصفح للتحميل
   - التحقق من إعدادات popup blocker

## 📝 ملاحظات مهمة

- النظام مصمم للعمل مع العمولات وليس الاشتراكات
- جميع الإيرادات تأتي من عمولات المهام المكتملة
- يمكن تخصيص طرق الدفع حسب الحاجة
- النظام يدعم اللغة العربية بالكامل

## 🔄 التحديثات المستقبلية

- إضافة المزيد من التقارير
- تحسين واجهة المستخدم
- إضافة إشعارات push
- تطوير تطبيق الهاتف المحمول

---

**تم تطوير النظام بواسطة:** فريق التطوير
**الإصدار:** 1.0.0
**تاريخ الإصدار:** 2024