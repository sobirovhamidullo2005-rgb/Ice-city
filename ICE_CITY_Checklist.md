# ICE CITY — Ilova Tekshiruv Cheklisti (QA Checklist)

> **Ilova:** ICE CITY  
> **Jarayon:** Foydalanuvchi onboarding flow (4 ta bog'liq ekran)  
> **Ekranlar ketma-ketligi:** Ekran 1 → Ekran 2 → Ekran 3 → Ekran 4

---

## 📱 EKRAN 1: Telefon raqam kiritish (Login)

| Title | Sub model | Description | Priority | Bugs | Bug type | Status | Notes |
|-------|-----------|-------------|----------|------|----------|--------|-------|
| Til tanlash — Russki | Login ekrani | "Русский" tugmasi bosilganda til rus tiliga o'tishi kerak | High | — | — | — | Til o'zgarishi barcha matnlarga ta'sir qilishi shart |
| Til tanlash — O'zbek tili | Login ekrani | "O'zbek tili" tugmasi bosilganda til o'zbek tiliga o'tishi kerak | High | — | — | — | Default til o'zbek bo'lishi kerak |
| Til tugmalari ko'rinishi | Login ekrani | Ikki tugma (bayroq + nom) to'g'ri ko'rinishi, faol til ajralib turishi | Medium | — | — | — | Faol til oq fonda, nofaol kulrang |
| Sarlavha matni | Login ekrani | "Xush kelibsiz!" matni to'g'ri til va shriftda ko'rinishi | Medium | — | — | — | — |
| Tavsif matni | Login ekrani | "Tizimga kirish uchun telefon raqamingizni kiriting" matni to'g'ri ko'rinishi | Medium | — | — | — | — |
| Telefon raqam maydoni | Login ekrani | "+998 __ __ __ __" placeholder to'g'ri formatda ko'rinishi | High | — | — | — | Faqat raqam kiritilishi kerak |
| Raqam kiritish — to'g'ri format | Login ekrani | +998 dan keyin 9 ta raqam kiritilganda format to'g'ri bo'lishi | High | — | — | — | Misol: +998 90 123 45 67 |
| Raqam kiritish — noto'g'ri format | Login ekrani | 9 tadan kam raqam kiritilganda xato xabari ko'rinishi | High | — | — | — | Xato xabari aniq va tushunarli bo'lsin |
| Raqam kiritish — harf kiritish | Login ekrani | Harflar kiritilganda qabul qilinmasligi kerak | High | — | — | — | Faqat raqam klaviaturasi chiqishi shart |
| "Davom etish" tugmasi — faol holat | Login ekrani | Raqam to'liq kiritilganda tugma faollashishi (ko'k rang) | High | — | — | — | — |
| "Davom etish" tugmasi — nofaol holat | Login ekrani | Raqam kiritilmagan yoki to'liq bo'lmasa tugma bosilmasligi | High | — | — | — | Tugma kulrang bo'lishi kerak |
| "Davom etish" tugmasi — bosilganda | Login ekrani | Tugma bosilganda Ekran 2 (SMS tasdiqlash) ga o'tishi | Critical | — | — | — | Navigatsiya to'g'ri ishlashi shart |
| Klaviatura chiqishi | Login ekrani | Telefon maydoni bosilganda raqamli klaviatura avtomatik chiqishi | Medium | — | — | — | — |
| Ekran joylashuvi | Login ekrani | Barcha elementlar ekranda to'g'ri joylashgan, kesib chiqmagan | Low | — | — | — | Turli ekran o'lchamlarida tekshirish |

---

## 📱 EKRAN 2: SMS tasdiqlash (OTP)

> ⚠️ **Bog'liqlik:** Ekran 1 dan telefon raqam kiritib "Davom etish" bosilgandan keyin ochiladi

| Title | Sub model | Description | Priority | Bugs | Bug type | Status | Notes |
|-------|-----------|-------------|----------|------|----------|--------|-------|
| Orqaga qaytish tugmasi | SMS tasdiqlash | "‹" tugmasi bosilganda Ekran 1 ga qaytishi | High | — | — | — | Kiritilgan raqam saqlanib qolishi kerak |
| Sarlavha matni | SMS tasdiqlash | "SMS tasdiqlash" matni to'g'ri ko'rinishi | Medium | — | — | — | — |
| Telefon raqam ko'rsatilishi | SMS tasdiqlash | "4 xonali kod yuborildi +99877 ***66" formatida raqam ko'rinishi | High | — | — | — | Raqam oxirgi 2 ta raqamdan tashqari yashirilgan bo'lishi shart |
| 4 ta OTP maydon | SMS tasdiqlash | 4 ta alohida maydon ko'rinishi va ishlashi | High | — | — | — | Har bir maydon 1 ta raqam qabul qiladi |
| OTP kiritish — avtomatik o'tish | SMS tasdiqlash | Har bir maydonga raqam kiritilganda keyingi maydonga avtomatik o'tishi | High | — | — | — | — |
| OTP kiritish — faqat raqam | SMS tasdiqlash | Harflar va belgilar qabul qilinmasligi | High | — | — | — | — |
| OTP kiritish — o'chirish (backspace) | SMS tasdiqlash | Backspace bosilganda oldingi maydonga qaytishi | Medium | — | — | — | — |
| OTP — to'g'ri kod | SMS tasdiqlash | To'g'ri 4 xonali kod kiritilganda Ekran 3 ga o'tishi | Critical | — | — | — | Navigatsiya to'g'ri ishlashi shart |
| OTP — noto'g'ri kod | SMS tasdiqlash | Noto'g'ri kod kiritilganda xato xabari ko'rinishi | High | — | — | — | Xato xabari aniq bo'lsin |
| Qayta yuborish — hisoblagich | SMS tasdiqlash | "Qayta yuborish: 56 sek" hisoblagichi ortga sanashi | High | — | — | — | 0 ga yetganda tugma faollashishi kerak |
| Qayta yuborish — tugma nofaol | SMS tasdiqlash | Hisoblagich 0 bo'lmasa tugma bosilmasligi | Medium | — | — | — | — |
| Qayta yuborish — tugma faol | SMS tasdiqlash | 0 ga yetganda "Qayta yuborish" tugmasi bosiladigan bo'lishi | Medium | — | — | — | — |
| Qayta yuborish — SMS kelishi | SMS tasdiqlash | Tugma bosilganda yangi SMS yuborilishi va hisoblagich qayta boshlanishi | High | — | — | — | — |
| "Davom etish" tugmasi — 4 raqam kiritilganda | SMS tasdiqlash | 4 ta raqam to'liq kiritilganda tugma faollashishi | High | — | — | — | — |
| "Davom etish" tugmasi — bosilganda | SMS tasdiqlash | Tugma bosilganda Ekran 3 ga o'tishi (agar kod to'g'ri) | Critical | — | — | — | — |
| SMS kelmasa | SMS tasdiqlash | Uzoq kutishda yoki xato raqamda foydalanuvchiga yo'riqnoma ko'rinishi | Medium | — | — | — | — |

---

## 📱 EKRAN 3: Ro'yxatdan o'tish (Profil)

> ⚠️ **Bog'liqlik:** Ekran 2 da OTP tasdiqlangandan keyin ochiladi

| Title | Sub model | Description | Priority | Bugs | Bug type | Status | Notes |
|-------|-----------|-------------|----------|------|----------|--------|-------|
| Orqaga qaytish tugmasi | Ro'yxatdan o'tish | "‹" tugmasi bosilganda Ekran 2 ga qaytishi | High | — | — | — | — |
| Sarlavha matni | Ro'yxatdan o'tish | "Ro'yxatdan o'tish" matni to'g'ri ko'rinishi | Medium | — | — | — | — |
| Rasm yuklash doirasi | Ro'yxatdan o'tish | "+" ikonasi bilan doira ko'rinishi | Medium | — | — | — | — |
| Rasm yuklash — bosilganda | Ro'yxatdan o'tish | Doira yoki "Rasm yuklash" bosilganda galereya/kamera ochilishi | High | — | — | — | — |
| Rasm yuklash — rasm tanlash | Ro'yxatdan o'tish | Rasm tanlanganda doirada profil rasmi ko'rinishi | High | — | — | — | — |
| Rasm yuklash — ruxsat so'rash | Ro'yxatdan o'tish | Galereya ruxsati so'ralganda to'g'ri tarzda so'ralishi | Medium | — | — | — | Android/iOS ruxsat tizimi |
| "Rasm yuklash" matni | Ro'yxatdan o'tish | Ko'k rangdagi "Rasm yuklash" matni ko'rinishi | Low | — | — | — | — |
| F.I.Sh maydoni | Ro'yxatdan o'tish | "F.I.Sh" placeholder bilan maydon ko'rinishi | High | — | — | — | — |
| F.I.Sh kiritish — to'g'ri | Ro'yxatdan o'tish | Ism, familiya, sharif kiritilganda qabul qilinishi | High | — | — | — | Kamida 2 so'z bo'lishi kerak |
| F.I.Sh kiritish — bo'sh | Ro'yxatdan o'tish | Bo'sh qoldirilsa xato xabari ko'rinishi | High | — | — | — | Majburiy maydon |
| F.I.Sh kiritish — faqat raqam | Ro'yxatdan o'tish | Faqat raqamdan iborat qiymat qabul qilinmasligi | Medium | — | — | — | — |
| Tug'ilgan sana maydoni | Ro'yxatdan o'tish | "Tug'ilgan sana" placeholder va taqvim ikonasi ko'rinishi | High | — | — | — | — |
| Tug'ilgan sana — taqvim ikonasi | Ro'yxatdan o'tish | Ikonaga bosiganda sana tanlash taqvimi ochilishi | High | — | — | — | — |
| Tug'ilgan sana — tanlash | Ro'yxatdan o'tish | Taqvimdan sana tanlab bo'lganda maydonda ko'rinishi | High | — | — | — | Format: KK.OO.YYYY |
| Tug'ilgan sana — bo'sh | Ro'yxatdan o'tish | Bo'sh qoldirilsa xato xabari ko'rinishi | High | — | — | — | Majburiy maydon |
| Tug'ilgan sana — kelajak sana | Ro'yxatdan o'tish | Kelajak sana tanlanmasligi kerak | High | — | — | — | — |
| Tug'ilgan sana — 18 yoshdan kam | Ro'yxatdan o'tish | 18 yoshdan kichik bo'lsa ogohlantirish yoki bloklash | Medium | — | — | — | Loyihaga qarab belgilansin |
| Jins tanlash — "Erkak" | Ro'yxatdan o'tish | "Erkak" radio tugmasi bosilganda tanlanishi | High | — | — | — | — |
| Jins tanlash — "Ayol" | Ro'yxatdan o'tish | "Ayol" radio tugmasi bosilganda tanlanishi | High | — | — | — | — |
| Jins tanlash — faqat bittasi | Ro'yxatdan o'tish | Bir vaqtda faqat bitta jins tanlanishi mumkin | High | — | — | — | — |
| Jins tanlash — bo'sh | Ro'yxatdan o'tish | Jins tanlanmasa xato xabari ko'rinishi | High | — | — | — | Majburiy maydon |
| "Tasdiqlash" tugmasi — faol | Ro'yxatdan o'tish | Barcha maydonlar to'ldirilganda tugma faollashishi (ko'k rang) | High | — | — | — | — |
| "Tasdiqlash" tugmasi — nofaol | Ro'yxatdan o'tish | Biror maydon bo'sh bo'lsa tugma bosilmasligi | High | — | — | — | — |
| "Tasdiqlash" tugmasi — bosilganda | Ro'yxatdan o'tish | Ma'lumotlar saqlangandan keyin Ekran 4 ga o'tishi | Critical | — | — | — | Navigatsiya to'g'ri ishlashi shart |
| Ma'lumotlar serverga yuborilishi | Ro'yxatdan o'tish | F.I.Sh, sana, jins, rasm serverga to'g'ri yuborilishi | Critical | — | — | — | API tekshiruvi |

---

## 📱 EKRAN 4: Virtual karta

> ⚠️ **Bog'liqlik:** Ekran 3 da "Tasdiqlash" bosilgandan keyin ochiladi

| Title | Sub model | Description | Priority | Bugs | Bug type | Status | Notes |
|-------|-----------|-------------|----------|------|----------|--------|-------|
| Orqaga qaytish tugmasi | Virtual karta | "‹" tugmasi bosilganda Ekran 3 ga qaytishi | High | — | — | — | — |
| Sarlavha matni | Virtual karta | "Virtual karta" matni to'g'ri ko'rinishi | Medium | — | — | — | — |
| 1-bandning ikonasi va matni | Virtual karta | Karta ikonasi + "Kartani onlayn oching yoki kassada olinganini yuklang" matni | Medium | — | — | — | — |
| 2-bandning ikonasi va matni | Virtual karta | Balans ikonasi + "Balansni to'ldiring — navbatsiz" matni | Medium | — | — | — | — |
| 3-bandning ikonasi va matni | Virtual karta | Chipta ikonasi + "Attraksionlarga chiptalarni to'g'ridan-to'g'ri ilovada sotib oling" matni | Medium | — | — | — | — |
| 4-bandning ikonasi va matni | Virtual karta | QR kod ikonasi + "Chipta QR kodini kirishda ko'rsating" matni | Medium | — | — | — | — |
| Bandlar ikonalari ko'rinishi | Virtual karta | Barcha 4 ta ikonani ko'k rangda va to'g'ri ko'rinishi | Low | — | — | — | — |
| Bandlar orasidagi chiziq | Virtual karta | Ikonalar orasidagi vertikal nuqtali chiziq to'g'ri ko'rinishi | Low | — | — | — | — |
| "Menda allaqachon karta bor" tugmasi | Virtual karta | Tugma ko'k matn bilan, och ko'k fonda ko'rinishi | High | — | — | — | — |
| "Menda allaqachon karta bor" — bosilganda | Virtual karta | Mavjud kartani bog'lash ekrani yoki jarayoni ochilishi | High | — | — | — | Keyingi flow bilan bog'liq |
| "Karta ochish" tugmasi | Virtual karta | Gradiyent ko'k tugma to'g'ri ko'rinishi | High | — | — | — | — |
| "Karta ochish" — bosilganda | Virtual karta | Yangi karta ochish jarayoni boshlanishi | Critical | — | — | — | — |
| Onboarding yakunlanishi | Virtual karta | Bu ekranda onboarding to'liq yakunlangan hisoblanadi | Critical | — | — | — | Foydalanuvchi tizimga kirgan |

---

## 🔗 OQIM (FLOW) TEKSHIRUVI — Barcha 4 ekran bog'liqligi

| Title | Sub model | Description | Priority | Bugs | Bug type | Status | Notes |
|-------|-----------|-------------|----------|------|----------|--------|-------|
| Ekran 1 → Ekran 2 o'tish | Flow | Raqam kiritib "Davom etish" bosilganda SMS ekrani ochilishi | Critical | — | — | — | — |
| Ekran 2 → Ekran 3 o'tish | Flow | To'g'ri OTP kiritilganda ro'yxatdan o'tish ekrani ochilishi | Critical | — | — | — | — |
| Ekran 3 → Ekran 4 o'tish | Flow | "Tasdiqlash" bosilganda virtual karta ekrani ochilishi | Critical | — | — | — | — |
| Ekran 2 → Ekran 1 qaytish | Flow | Ekran 2 dan "‹" bosilganda Ekran 1 ga qaytishi, raqam saqlanishi | High | — | — | — | — |
| Ekran 3 → Ekran 2 qaytish | Flow | Ekran 3 dan "‹" bosilganda Ekran 2 ga qaytishi | High | — | — | — | — |
| Ekran 4 → Ekran 3 qaytish | Flow | Ekran 4 dan "‹" bosilganda Ekran 3 ga qaytishi | High | — | — | — | — |
| Internet yo'q holati | Flow | Internet yo'q bo'lganda har bir ekranda xato xabari ko'rinishi | High | — | — | — | — |
| Seans muddati tugashi | Flow | Uzoq kutilganda sessiya muddati tugashi va qayta kirish so'ralishi | Medium | — | — | — | — |
| Ilovani yopib qayta ochish | Flow | Jarayon o'rtasida ilova yopilsa, qayta ochilganda to'g'ri ekran ko'rinishi | Medium | — | — | — | — |
| Orqaga tugmasi (telefon) | Flow | Telefon orqaga tugmasi har bir ekranda to'g'ri ishlashi | High | — | — | — | Android fizik tugma |

---

## 📊 STATUS TURLARI

| Status | Ma'nosi |
|--------|---------|
| ✅ Pass | Tekshirildi, xato yo'q |
| ❌ Fail | Xato topildi |
| ⏳ In Progress | Tekshirilmoqda |
| ⏭️ Skip | O'tkazib yuborildi |
| 🔄 Retest | Qayta tekshirish kerak |

## 🐛 BUG TYPE TURLARI

| Bug type | Ma'nosi |
|----------|---------|
| UI | Ko'rinish xatosi |
| Functional | Funksional xato |
| Navigation | Navigatsiya xatosi |
| Validation | Tekshiruv xatosi |
| Performance | Ishlash tezligi xatosi |
| Crash | Ilova to'xtab qolishi |
| Network | Tarmoq xatosi |

## ⚡ PRIORITY TURLARI

| Priority | Ma'nosi |
|----------|---------|
| Critical | Darhol tuzatilishi shart, flow bloklangan |
| High | Muhim, tezda tuzatilishi kerak |
| Medium | O'rta muhimlikdagi xato |
| Low | Kichik xato, keyinroq tuzatilishi mumkin |
