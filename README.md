# CATO Premium Landing Page

Премиум лендинг для приложения CATO с современными анимациями и scroll-эффектами.

## 🎨 Особенности дизайна

- ✨ Современный минималистичный дизайн
- 🎬 Плавные scroll-анимации и параллакс эффекты
- 🌐 Полная мультиязычность (RU, ҚАЗ, EN)
- 📱 100% адаптивный дизайн
- 🎯 Интерактивные элементы
- 🔥 Premium UI/UX

## 🚀 Технологии

- **HTML5** - Семантическая разметка
- **CSS3** - Modern CSS с Grid, Flexbox, Custom Properties
- **JavaScript ES6+** - Vanilla JS без зависимостей
- **Font Awesome** - Иконки
- **Google Fonts** - Inter & Playfair Display
- **Canvas API** - Интерактивные частицы

## 📦 Структура

```
cato-premium/
├── index.html              # Главная страница
├── style.css              # Стили с анимациями
├── script.js              # JavaScript функционал
├── assets/
│   ├── splash.png         # Splash screen
│   ├── images/            # Дополнительные изображения
│   └── icons/             # Иконки
└── README.md              # Документация
```

## 🎯 Секции лендинга

### 1. Hero Section
- Крупный анимированный заголовок
- Coming Soon badge с плавающей анимацией
- Splash изображение приложения
- Статистика (рестораны, пользователи, рейтинг)
- CTA кнопки
- Интерактивные частицы на Canvas

### 2. Features Section
- 6 карточек с ключевыми возможностями
- Hover эффекты с трансформацией
- Градиентные иконки
- Плавное появление при скролле

### 3. How It Works Section
- 4 шага использования приложения
- Альтернирующий layout
- Анимированные номера шагов
- Иконки для каждого шага

### 4. Benefits Section
- 6 преимуществ CATO
- Центрированные карточки
- Круглые иконки с градиентом
- Grid layout с адаптивностью

### 5. Social Proof Section
- Бегущая строка с логотипами партнеров
- Темный фон для контраста
- Infinite loop анимация
- Hover эффекты

### 6. CTA Section
- Яркий градиентный фон
- Форма подписки
- App Store / Google Play badges
- Анимированный паттерн на фоне

### 7. Footer
- 4-колоночный layout
- Социальные сети
- Навигационные ссылки
- Темный дизайн

## 🎨 Цветовая палитра

```css
--primary: #FF4F00        /* Оранжевый (основной) */
--primary-dark: #E64500   /* Темно-оранжевый */
--primary-light: #FF6B2B  /* Светло-оранжевый */
--secondary: #1A1A1A      /* Темно-серый */
--text: #0A0A0A          /* Черный текст */
--text-light: #666666     /* Светло-серый текст */
--bg: #FAFAFA            /* Светлый фон */
--bg-alt: #FFFFFF        /* Белый фон */
```

## ⚡ Анимации и эффекты

### Scroll Animations
- Reveal эффект для элементов при скролле
- Parallax для hero изображения
- Плавное появление карточек с задержкой

### Interactive Elements
- Custom cursor с follower
- Hover эффекты на кнопках и карточках
- Floating badge анимация
- Infinite marquee для партнеров

### Canvas Particles
- 80 частиц с физикой движения
- Соединение близких частиц линиями
- Адаптивность к размеру экрана

### Transitions
- Cubic-bezier для плавности
- Transform-based анимации для производительности
- CSS transitions для hover эффектов

## 🌐 Мультиязычность

Переключение языков через кнопки в навигации:
- 🇷🇺 **RU** - Русский (по умолчанию)
- 🇰🇿 **ҚАЗ** - Қазақша
- 🇬🇧 **EN** - English

Все тексты хранятся в объекте `translations` в `script.js`.

### Добавление нового языка

```javascript
const translations = {
  // ... existing languages
  es: {
    nav_features: "Características",
    // ... add all keys
  }
};
```

## 📱 Адаптивность

### Breakpoints
- **Desktop**: 1200px+
- **Tablet**: 768px - 1199px
- **Mobile**: 320px - 767px

### Адаптивные элементы
- Grid → Flex → Stack
- Hero layout меняется на мобильных
- Навигация превращается в hamburger menu
- Уменьшение размеров шрифтов
- Оптимизация отступов

## 🚀 Запуск

### Локально
Просто откройте `index.html` в браузере.

### С сервером

```bash
# Python
python -m http.server 8000

# Node.js
npx http-server

# PHP
php -S localhost:8000
```

Затем откройте `http://localhost:8000`

## ⚙️ Настройка

### Изменение цветов

Отредактируйте CSS переменные в `:root`:

```css
:root {
  --primary: #FF4F00;
  --primary-dark: #E64500;
  /* ... */
}
```

### Добавление секции

1. Добавьте HTML разметку
2. Добавьте стили в `style.css`
3. Добавьте переводы в `script.js`
4. Добавьте scroll reveal если нужно

### Замена изображений

1. Поместите изображения в `assets/images/`
2. Замените пути в HTML
3. Оптимизируйте для веба (WebP рекомендуется)

## 🎯 Оптимизация

### Производительность
- ✅ CSS transform вместо position/size
- ✅ RequestAnimationFrame для анимаций
- ✅ Debounce для scroll events
- ✅ Lazy loading для изображений

### SEO
- ✅ Семантические HTML теги
- ✅ Meta теги для соцсетей
- ✅ Alt атрибуты для изображений
- ✅ Структурированные данные

### Accessibility
- ✅ Правильная иерархия заголовков
- ✅ ARIA атрибуты
- ✅ Keyboard navigation
- ✅ Цветовой контраст

## 🌟 Браузерная поддержка

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 📝 Чеклист для production

- [ ] Минифицировать CSS и JS
- [ ] Оптимизировать изображения (WebP)
- [ ] Добавить loading states
- [ ] Настроить CDN для статики
- [ ] Добавить Google Analytics
- [ ] Настроить мета теги для каждого языка
- [ ] Протестировать на реальных устройствах
- [ ] Добавить Service Worker для PWA

## 🤝 Вклад

Для внесения изменений:
1. Создайте feature branch
2. Внесите изменения
3. Протестируйте на всех устройствах
4. Создайте pull request

## 📄 Лицензия

© 2026 CATO Inc. Все права защищены.

## 📧 Контакты

- Email: info@cato.app
- Website: https://cato.app
- Instagram: @cato.app
- Telegram: @cato_support

---

Made with ❤️ by CATO Team
