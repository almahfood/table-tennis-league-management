# 🏓 منصة إدارة مسابقات الاتحاد البحريني لكرة الطاولة

## 📋 نظرة عامة

منصة رقمية شاملة لإدارة مسابقات الاتحاد البحريني لكرة الطاولة، توفر نظاماً متكاملاً لتسجيل اللاعبين والأندية والحكام والمباريات والدوري العام بكافة فئاته.

## ✨ المميزات الرئيسية

### 1️⃣ إدارة الأندية
- ✅ تسجيل الأندية الرسمية
- ✅ إدارة بيانات الأندية (اسم، عنوان، اتصالات)
- ✅ تتبع عدد اللاعبين في كل نادي
- ✅ إدارة مديري الأندية

### 2️⃣ إدارة اللاعبين
- ✅ تسجيل اللاعبين الجدد
- ✅ ربط اللاعبين بالأندية
- ✅ إدارة البيانات الشخصية
- ✅ تتبع إحصائيات اللاعب
- ✅ نظام التصنيف والترتيب

### 3️⃣ إدارة الحكام
- ✅ تسجيل الحكام المعتمدين
- ✅ تحديد مستويات الحكام
- ✅ تعيين الحكام للمباريات
- ✅ تقييم أداء الحكام

### 4️⃣ إدارة المباريات
- ✅ جدولة المباريات
- ✅ تسجيل نتائج المباريات
- ✅ إدارة تفاصيل المباريات
- ✅ تحديث الترتيب تلقائياً

### 5️⃣ الدوري العام
- ✅ إنشاء فئات مختلفة
- ✅ جدول الدوري والترتيبات
- ✅ إحصائيات شاملة
- ✅ جوائز ونتائج نهائية

### 6️⃣ لوحة التحكم الإدارية
- ✅ لوحة تحكم شاملة
- ✅ تقارير مفصلة
- ✅ إحصائيات الدوري
- ✅ إدارة المستخدمين

## 🏗️ البنية التكنولوجية

```
table-tennis-league-management/
├── frontend/                    # تطبيق الويب (React/Vue)
│   ├── public/
│   ├── src/
│   │   ├── components/         # مكونات React
│   │   ├── pages/              # صفحات التطبيق
│   │   ├── services/           # خدمات API
│   │   ├── hooks/              # React Hooks
│   │   └── styles/             # التصاميم
│   └── package.json
│
├── backend/                     # API الخادم (Flask/Django)
│   ├── app/
│   │   ├── models/             # نماذج قاعدة البيانات
│   │   ├── controllers/        # معالجات الطلبات
│   │   ├── routes/             # طرق API
│   │   ├── middleware/         # Middleware
│   │   ├── services/           # خدمات الأعمال
│   │   └── utils/              # دوال مساعدة
│   ├── database/
│   │   ├── migrations/         # ترقيات قاعدة البيانات
│   │   └── seeds/              # بيانات اختبار
│   ├── tests/                  # اختبارات الوحدة
│   └── requirements.txt
│
├── database/                    # ملفات قاعدة البيانات
│   ├── schema.sql              # هيكل الجداول
│   └── indexes.sql             # الفهارس
│
├── docs/                        # التوثيق
│   ├── API.md                  # توثيق API
│   ├── DATABASE.md             # توثيق قاعدة البيانات
│   ├── SETUP.md                # دليل التثبيت
│   └── ARCHITECTURE.md         # معمارية النظام
│
├── nginx/                       # إعدادات Nginx
├── .github/workflows/          # CI/CD Workflows
├── .gitignore
├── .env.example
├── docker-compose.yml
├── Dockerfile
└── README.md
```

## 🛠️ التقنيات المستخدمة

### Backend
- **Python 3.9+**
- **Flask** أو **Django** لـ REST API
- **PostgreSQL** لقاعدة البيانات
- **Redis** للـ Caching
- **JWT** للمصادقة
- **SQLAlchemy** لـ ORM

### Frontend
- **React.js** أو **Vue.js 3**
- **Tailwind CSS** أو **Bootstrap 5** للتصميم
- **Axios** للـ HTTP Requests
- **Redux/Vuex** لإدارة الحالة
- **Chart.js** للإحصائيات

### DevOps
- **Docker** و **Docker Compose**
- **Nginx** كـ Reverse Proxy
- **GitHub Actions** للـ CI/CD
- **PostgreSQL Backups**

## 🚀 البدء السريع

### المتطلبات الأساسية

```bash
- Git
- Docker و Docker Compose
- أو Python 3.9+ و Node.js 16+
```

### الخيار 1: استخدام Docker (الموصى به)

```bash
# 1. استنساخ المستودع
git clone https://github.com/almahfood/table-tennis-league-management.git
cd table-tennis-league-management

# 2. نسخ ملف المتغيرات البيئية
cp .env.example .env

# 3. تشغيل البيئة
docker-compose up -d

# 4. الوصول للتطبيق
# Frontend: http://localhost:3000
# Backend: http://localhost:5000
# Database: localhost:5432
```

### الخيار 2: التثبيت اليدوي

#### إعداد Backend

```bash
cd backend

# إنشاء بيئة افتراضية
python -m venv venv
source venv/bin/activate  # على Windows: venv\Scripts\activate

# تثبيت المتطلبات
pip install -r requirements.txt

# إعداد قاعدة البيانات
flask db upgrade

# تشغيل الخادم
python app.py
```

#### إعداد Frontend

```bash
cd frontend

# تثبيت المكتبات
npm install

# تشغيل التطبيق
npm start
```

## 📊 الوصول للتطبيق

| الخدمة | الرابط | المنفذ |
|------|-------|--------|
| 🌐 Frontend | http://localhost:3000 | 3000 |
| 🔌 Backend API | http://localhost:5000 | 5000 |
| 🗄️ Database | localhost:5432 | 5432 |
| 💾 Redis Cache | localhost:6379 | 6379 |

## 📚 التوثيق الكاملة

- 📖 [API Documentation](./docs/API.md) - جميع نقاط نهاية API
- 🗄️ [Database Schema](./docs/DATABASE.md) - هيكل قاعدة البيانات
- 🔧 [Setup Guide](./docs/SETUP.md) - دليل التثبيت المفصل
- 🏗️ [Architecture](./docs/ARCHITECTURE.md) - معمارية النظام
- 🤝 [Contributing Guide](./CONTRIBUTING.md) - دليل المساهمة

## 👥 الأدوار والصلاحيات

| الدور | الوصف | الصلاحيات |
|------|-------|---------|
| 👨‍💼 **Admin** | مسؤول النظام | إدارة كاملة |
| 🏢 **Manager** | مدير النادي | إدارة اللاعبين والمباريات |
| 🎯 **Referee** | حكم المباراة | تسجيل النتائج والنقاط |
| 👤 **User** | مستخدم عادي | عرض الترتيبات والإحصائيات |

## 🔐 الأمان

- 🔒 تشفير كلمات المرور (bcrypt)
- 🎫 JWT للمصادقة
- 🔐 HTTPS/TLS
- 🛡️ حماية CSRF
- ✅ التحقق من الصلاحيات
- 📝 Audit Logs
- 🔄 نسخ احتياطية منتظمة

## 📈 الإحصائيات المدعومة

- 📊 إحصائيات اللاعب (الفوز، الخسارة، النسبة المئوية)
- 🏆 ترتيب الدوري
- 📈 تطور الأداء
- 🎯 إحصائيات الحكام
- 👥 إحصائيات الأندية

## 🧪 الاختبارات

### تشغيل الاختبارات

```bash
# اختبارات Backend
cd backend
pytest tests/

# اختبارات Frontend
cd frontend
npm test
```

### تغطية الاختبارات

```bash
pytest --cov=app tests/
```

## 📦 المتطلبات

### Backend (requirements.txt)
```
Flask==2.3.2
Flask-SQLAlchemy==3.0.3
Flask-JWT-Extended==4.4.4
psycopg2-binary==2.9.6
Redis==4.5.5
python-dotenv==1.0.0
pytest==7.3.1
```

### Frontend (package.json)
```json
{
  "dependencies": {
    "react": "^18.2.0",
    "react-router-dom": "^6.11.0",
    "axios": "^1.4.0",
    "tailwindcss": "^3.3.0"
  }
}
```

## 📞 التواصل والدعم

- 📧 **البريد الإلكتروني**: support@table-tennis-bh.org
- 📱 **الهاتف**: +973 XXXX XXXX
- 🌐 **الموقع**: www.table-tennis-bh.org
- 💬 **مناقشات GitHub**: [GitHub Discussions](https://github.com/almahfood/table-tennis-league-management/discussions)

## 📄 الترخيص

هذا المشروع مرخص تحت **MIT License** - انظر ملف [LICENSE](./LICENSE)

## 🙏 شكر وتقدير

شكراً للاتحاد البحريني لكرة الطاولة على دعمهم لهذا المشروع.

## 🤝 المساهمة

نرحب بالمساهمات من جميع المطورين! 

### كيفية المساهمة:
1. اقرأ [CONTRIBUTING.md](./CONTRIBUTING.md)
2. Fork المستودع
3. أنشئ فرع جديد لميزتك
4. Commit التغييرات
5. Push وفتح Pull Request

---

<div align="center">

**صُنع بـ ❤️ من قبل فريق التطوير**

**آخر تحديث**: سبتمبر 2026 | **الإصدار**: 1.0.0-beta

</div>
