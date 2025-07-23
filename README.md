# wishlist-frontend

wishlist-frontend/
├── src/
│   ├── app/
│   │   ├── core/               # Глобальные компоненты
│   │   │   ├── services/
│   │   │   │   ├── api.service.ts         # HTTP клиент
│   │   │   │   ├── auth.service.ts        # login(), register(), logout()
│   │   │   │   ├── wish.service.ts        # getWishes(), createWish()
│   │   │   │   └── auth.interceptor.ts    # Добавляет токен к запросам
│   │   │   ├── guards/
│   │   │   │   └── auth.guard.ts          # Защита роутов
│   │   │   ├── models/         # Типы данных
│   │   │   │   ├── user.model.ts
│   │   │   │   ├── wish.model.ts
│   │   │   │   └── category.model.ts
│   │   │   └── utils/          # Вспомогательные функции
│   │   │       └── api-url.const.ts
│   │   │
│   │   ├── modules/            # Feature модули
│   │   │   ├── auth/
│   │   │   │   ├── login/      # Компонент логина
│   │   │   │   ├── register/   # Компонент регистрации
│   │   │   │   └── auth-routing.module.ts
│   │   │   │
│   │   │   ├── wishes/
│   │   │   │   ├── wish-list/  # Список желаний
│   │   │   │   ├── wish-detail/# Детали желания
│   │   │   │   ├── wish-edit/  # Редактор
│   │   │   │   └── wishes-routing.module.ts
│   │   │   │
│   │   │   └── shared/         # Общие компоненты
│   │   │       ├── components/
│   │   │       │   ├── header/ # Шапка с меню
│   │   │       │   ├── loader/ # Индикатор загрузки
│   │   │       │   └── wish-card/ # Карточка желания
│   │   │       ├── pipes/
│   │   │       └── directives/
│   │   │
│   │   ├── app-routing.module.ts # Главная маршрутизация
│   │   ├── app.component.ts
│   │   └── app.module.ts        # Корневой модуль
│   │
│   ├── assets/
│   ├── environments/            # Конфиги для dev/prod
│   └── styles/                  # Глобальные стили
│
├── angular.json
└── package.json