# CyberSentinel: Splunk Security Analytics

![Tool](https://img.shields.io/badge/Tool-Splunk-blue) ![Status](https://img.shields.io/badge/Status-Completed-brightgreen) ![Category](https://img.shields.io/badge/Threat_Investigation-red)

## سيناريو التحقيق الأمني (The Investigation Story)
في هذا المشروع، أتقمص دور **محلل أمن سيبراني (SOC Analyst)** يواجه سلسلة من محاولات اختراق مشبوهة. بدأت القصة بظهور ارتفاع غير مبرر في سجلات فشل تسجيل الدخول، مما دفعني لفتح تحقيق جنائي رقمي باستخدام Splunk للكشف عن هوية المهاجم وتأمين الأصول الرقمية للشركة.

---

## المرحلة الأولى: الاستطلاع وتحليل البيئة (Phase 1: Recon & Ingestion)
بدأتُ الرحلة بتهيئة البيئة وفهم حجم التهديد الذي أواجهه.
* **Environment Setup & Source Analysis:** ![Setup](screenshots/environment-setup.png) ![Source](screenshots/data-source.png)
*شرح: تهيئة الفهارس للتأكد من أننا نرى الصورة الكاملة للهجوم.*
* **Ingestion Overview:** ![Volume](screenshots/data-volume.png) ![Count](screenshots/ingestion-count.png)
*شرح: التأكد من تدفق البيانات لضمان عدم وجود "بقع عمياء" في رصدنا.*

---

## المرحلة الثانية: مطاردة المهاجم (Phase 2: The Hunt)
استخدمتُ لغة SPL لتحويل السجلات الصامتة إلى أدلة ملموسة.
* **Log Inspection & Auth Failures:** ![Logs](screenshots/raw-logs.png) ![General](screenshots/auth-failure-query.png)
*شرح: تحليل سجلات 4625. اكتشفتُ نمطاً متكرراً يشير بوضوح إلى هجوم Brute-Force.*
* **Precision SPL Detection:** ![SPL](screenshots/brute-force-spl.png)
*شرح: صياغة استعلام ذكي لاكتشاف المحاولات الأكثر كثافة ومحاصرة المهاجم.*

---

## المرحلة الثالثة: التحليل الجنائي (Phase 3: Forensic Findings)
هنا بدأت أربط النقاط ببعضها وأفهم "من" و"ماذا" استهدفوا.
* **IP Activity & Attacker Identity:** ![IPs](screenshots/top-ips.png) ![Map](screenshots/ip-activity.png) ![Attacker](screenshots/attacker-id.png)
*شرح: تحديد عناوين الـ IP المهاجمة ورسم خرائط زمنية لنشاطهم.*
* **Targeted Account Analysis:** ![Targeted](screenshots/targeted-accounts.png) ![Viz](screenshots/compromised-accounts.png)
*شرح: اكتشاف الحسابات الحساسة التي حاول المهاجم الوصول إليها وتقديم تقرير بها.*

---

## المرحلة الرابعة: الاستجابة والتحصين (Phase 4: Response & Defense)
لا يكفي الكشف، يجب أن نغلق الأبواب ونراقب في المستقبل.
* **SOC Dashboard & Alerting:** ![Dashboard](screenshots/soc-dashboard.png) ![Details](screenshots/alert-details.png)
*شرح: بناء واجهة تحكم لحظية تضعني في قلب الحدث.*
* **Automated Alerting Workflow:** ![Workflow](screenshots/alert-workflow.png) ![Active](screenshots/active-alerts.png)
*شرح: "السيناريو الدفاعي": برمجة تنبيهات تعمل كل ساعة لرصد أي محاولة تكرار للهجوم فور وقوعها.*

---

## الخاتمة (Closing the Case)
تم إغلاق التحقيق بعد تحديد المصادر المهاجمة وتفعيل إجراءات الصد. لقد حولنا السجلات الخام إلى "معلومات استخباراتية" (Threat Intel) تحمي المنظمة.

