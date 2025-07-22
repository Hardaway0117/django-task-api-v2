# Django Task API v2

這是一個使用 Django REST Framework 建立的任務管理系統 API，支援完整的 CRUD 功能與進階查詢

## 🧩 主要功能

- ✅ 任務建立 / 查詢 / 修改 / 刪除（CRUD）含後台
- 🔍 支援條件篩選：狀態、是否完成、建立日期區間
- 🔎 支援模糊搜尋與排序功能（Search + Ordering Filter）
- 📄 分頁功能（每頁筆數可調整）
- 🔐 使用者與任務關聯（透過 ForeignKey）
- 🛠 管理員後台（Django Admin）
superuser >> (http://127.0.0.1:8000/admin/)

## 📦 安裝步驟

```bash
git clone https://github.com/Hardaway0117/django-task-api-v2.git
cd django-task-api-v2
python -m venv venv
venv\\Scripts\\activate           # Mac/Linux 使用 source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser  # 建立管理員帳號（可登入 /admin）
python manage.py runserver
