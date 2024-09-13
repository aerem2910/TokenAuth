

# Доработка домашнего задания 

Внесены следующие изменения в программу:

1. **Токен идентификации пользователя:**
   - В токен идентификации пользователя (в классе `TokenService`) были добавлены дополнительные данные, такие как ID пользователя и другие метаданные. Это позволяет более подробно описать пользователя в токене, что может быть полезно для GraphQL API.

2. **Обработка ошибок и результатов в сервисе аутентификации:**
   - В методе `Login` класса `AuthService` были внесены изменения для использования пользовательских исключений (`UserNotFoundException` и `InvalidCredentialsException`). Это облегчает обработку идентификации в GraphQL-запросах и предоставляет более информативные ошибки.

3. **Интерфейс ITokenService:**
   - В интерфейсе `ITokenService` была обновлена сигнатура метода `GenerateToken`, чтобы включить ID пользователя и другие метаданные в токен. Это позволяет интерфейсу лучше соответствовать реализации.

Эти изменения улучшают функциональность аутентификации и предоставляют дополнительные данные в токене для использования в GraphQL API. 
