# F.R.I.D.A.Y. OS Mobile — Stage 1

Первый Android-проект F.R.I.D.A.Y. OS Mobile. Это приложение-прототип, а не замена Android.

## Возможности
- Футуристический тёмный интерфейс.
- Проверка `GET /health`.
- Чат через `POST /chat` с JSON `{"message":"..."}`.
- Понятный вывод ошибок HTTP/API.
- Секретный HF_TOKEN хранится только на backend; в приложении токены не нужны.

## Backend
`https://friday-ai-backend-gfc4.onrender.com`

## Сборка APK на Windows
1. Установи Android Studio с Android SDK и JDK 17.
2. Распакуй архив.
3. Открой в Android Studio папку `FRIDAY_OS_Mobile_Stage1`.
4. Дождись Gradle Sync.
5. Если Android Studio попросит установить Android SDK Platform 35, согласись.
6. Выбери **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
7. APK появится в `app/build/outputs/apk/debug/app-debug.apk`.

## Важно
- Для сборки нужен интернет и Android Studio/Gradle.
- Я не могу подтвердить сборку APK в этом окружении; архив содержит исходный Android-проект.
- Если сервер вернёт 502, это ошибка backend/языковой модели, не мобильного интерфейса.
- Не помещай HF_TOKEN в приложение или GitHub.
