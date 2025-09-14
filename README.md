## О проекте

Services.VPN - сервис VPN для модульного P&Z Apps Hub приложения. Реализует функционал виртуальной частной сети с поддержкой различных протоколов, управлением подключениями, мониторингом трафика и обеспечением безопасности. Поддерживает multiple VPN protocols и provides secure tunneling capabilities.

## Структура проекта

```
Services.VPN/
├── Services/               # Реализации VPN сервисов
│   ├── VpnConnectionService.cs  # Основной сервис подключений
│   ├── VpnServerService.cs      # Сервис управления серверами
│   ├── VpnSecurityService.cs    # Сервис безопасности
│   ├── VpnMonitoringService.cs  # Сервис мониторинга
│   ├── VpnConfigurationService.cs # Сервис конфигурации
│   └── VpnProtocolService.cs    # Сервис поддержки протоколов
├── Models/                 # Модели данных VPN
│   ├── VpnServer.cs           # VPN сервер
│   ├── VpnConnection.cs       # VPN подключение
│   ├── VpnConfiguration.cs    # Конфигурация VPN
│   ├── VpnStatistics.cs       # Статистика трафика
│   ├── VpnCertificate.cs      # Сертификат безопасности
│   └── VpnProtocolSettings.cs # Настройки протоколов
├── Protocols/              # Реализации VPN протоколов
│   ├── OpenVpnService.cs      # OpenVPN implementation
│   ├── WireGuardService.cs    # WireGuard implementation
│   ├── L2tpService.cs         # L2TP/IPsec implementation
│   ├── SstpService.cs         # SSTP implementation
│   └── IVpnProtocol.cs        # Интерфейс протокола
├── Managers/               # Менеджеры управления
│   ├── ConnectionManager.cs    # Менеджер подключений
│   ├── ServerManager.cs        # Менеджер серверов
│   ├── CertificateManager.cs   # Менеджер сертификатов
│   └── RouteManager.cs         # Менеджер маршрутизации
├── Security/               # Компоненты безопасности
│   ├── EncryptionService.cs    # Сервис шифрования
│   ├── CertificateService.cs   # Сервис сертификатов
│   ├── AuthenticationService.cs # Сервис аутентификации
│   └── FirewallService.cs      # Фаервол сервис
├── Monitoring/             # Мониторинг и аналитика
│   ├── TrafficMonitor.cs       # Монитор трафика
│   ├── ConnectionMonitor.cs    # Монитор подключений
│   ├── PerformanceMonitor.cs   # Монитор производительности
│   └── UsageStatistics.cs      # Статистика использования
├── DTOs/                   # DTO для VPN
│   ├── VpnConnectionRequest.cs # Запрос подключения
│   ├── VpnServerResponse.cs    # Ответ с сервером
│   ├── VpnStatisticsResponse.cs # Ответ со статистикой
│   └── VpnConfigResponse.cs    # Ответ с конфигурацией
└── Utilities/              # Вспомогательные утилиты
    ├── ConfigGenerators/      # Генераторы конфигураций
    ├── NetworkUtilities/      # Сетевые утилиты
    ├── CertificateGenerators/ # Генераторы сертификатов
    └── ProtocolHandlers/      # Обработчики протоколов
```
