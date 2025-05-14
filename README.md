# Wiggle Website Test Automation Framework

## Task 4: BDD Framework Implementation

This task implements a Behavior-Driven Development (BDD) framework for testing the Wiggle website (https://www.wiggle.com/). The framework is built using:
- Java
- Selenium WebDriver
- Cucumber
- Maven

### Project Structure
```
src/
├── main/java/com/wiggle/
│   ├── factory/
│   │   └── WebDriverFactory.java
│   └── pages/
│       ├── BasePage.java
│       ├── HomePage.java
│       └── LoginPage.java
└── test/
    ├── java/com/wiggle/
    │   ├── runners/
    │   │   └── TestRunner.java
    │   └── steps/
    │       └── LoginSteps.java
    └── resources/features/
        └── login.feature
```

### Key Components
1. **WebDriverFactory**: Manages browser instances and configurations
2. **BasePage**: Contains common functionality for all page objects
3. **Page Objects**: Implement the Page Object pattern for better maintainability
4. **Feature Files**: Define test scenarios in Gherkin syntax
5. **Step Definitions**: Implement the behavior described in feature files

### Test Scenarios
The framework includes comprehensive test scenarios for:
- Login functionality
- Session management
- Form validation
- Security features
- User interactions

## Task 5: Defects and Improvements Testing

This task focuses on identifying and testing potential defects and improvements for the Wiggle website. The implementation includes 20 different test cases covering various aspects of the website.

### Test Categories
1. **Accessibility Testing**
   - Alt text verification for images
   - Color contrast compliance

2. **Performance Testing**
   - Page load time measurement
   - Memory usage monitoring

3. **Usability Testing**
   - Mobile responsiveness
   - Search functionality

4. **Security Testing**
   - Password strength validation
   - Session management

5. **Functional Testing**
   - Product comparison
   - Wishlist features

6. **Compatibility Testing**
   - Cross-browser validation
   - Responsive design

7. **Content Testing**
   - Product descriptions
   - Information architecture

8. **Integration Testing**
   - Social media sharing
   - Payment processing

9. **Navigation Testing**
   - Breadcrumb functionality
   - Menu organization

10. **Data Management Testing**
    - Stock updates
    - Price consistency

### Implementation Details
- Uses BDD approach with Cucumber
- Implements Page Object pattern
- Includes comprehensive assertions
- Handles different browser states
- Supports parallel test execution

## How to Run Tests
1. Clone the repository
2. Install dependencies: `mvn clean install`
3. Run all tests: `mvn test`
4. Run specific test categories: `mvn test -Dcucumber.filter.tags="@accessibility"`

---

# Фреймворк автоматизации тестирования сайта Wiggle

## Задание 4: Реализация BDD фреймворка

Это задание реализует фреймворк для тестирования на основе Behavior-Driven Development (BDD) для сайта Wiggle (https://www.wiggle.com/). Фреймворк построен с использованием:
- Java
- Selenium WebDriver
- Cucumber
- Maven

### Структура проекта
```
src/
├── main/java/com/wiggle/
│   ├── factory/
│   │   └── WebDriverFactory.java
│   └── pages/
│       ├── BasePage.java
│       ├── HomePage.java
│       └── LoginPage.java
└── test/
    ├── java/com/wiggle/
    │   ├── runners/
    │   │   └── TestRunner.java
    │   └── steps/
    │       └── LoginSteps.java
    └── resources/features/
        └── login.feature
```

### Основные компоненты
1. **WebDriverFactory**: Управляет экземплярами браузера и их конфигурацией
2. **BasePage**: Содержит общую функциональность для всех page objects
3. **Page Objects**: Реализует паттерн Page Object для лучшей поддерживаемости
4. **Feature Files**: Определяют тестовые сценарии в синтаксисе Gherkin
5. **Step Definitions**: Реализуют поведение, описанное в feature files

### Тестовые сценарии
Фреймворк включает комплексные тестовые сценарии для:
- Функциональности входа в систему
- Управления сессиями
- Валидации форм
- Функций безопасности
- Взаимодействия с пользователем

## Задание 5: Тестирование дефектов и улучшений

Это задание фокусируется на выявлении и тестировании потенциальных дефектов и улучшений для сайта Wiggle. Реализация включает 20 различных тестовых случаев, охватывающих различные аспекты сайта.

### Категории тестирования
1. **Тестирование доступности**
   - Проверка альтернативного текста для изображений
   - Соответствие контрастности цветов

2. **Тестирование производительности**
   - Измерение времени загрузки страницы
   - Мониторинг использования памяти

3. **Тестирование удобства использования**
   - Адаптивность для мобильных устройств
   - Функциональность поиска

4. **Тестирование безопасности**
   - Валидация надежности пароля
   - Управление сессиями

5. **Функциональное тестирование**
   - Сравнение продуктов
   - Функции списка желаний

6. **Тестирование совместимости**
   - Кросс-браузерная валидация
   - Адаптивный дизайн

7. **Тестирование контента**
   - Описания продуктов
   - Информационная архитектура

8. **Тестирование интеграции**
   - Шеринг в социальных сетях
   - Обработка платежей

9. **Тестирование навигации**
   - Функциональность хлебных крошек
   - Организация меню

10. **Тестирование управления данными**
    - Обновления запасов
    - Согласованность цен

### Детали реализации
- Использует подход BDD с Cucumber
- Реализует паттерн Page Object
- Включает комплексные проверки
- Обрабатывает различные состояния браузера
- Поддерживает параллельное выполнение тестов

## Как запустить тесты
1. Клонировать репозиторий
2. Установить зависимости: `mvn clean install`
3. Запустить все тесты: `mvn test`
4. Запустить определенные категории тестов: `mvn test -Dcucumber.filter.tags="@accessibility"` 