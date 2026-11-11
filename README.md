# GitHub-квиз
[![CI](https://github.com/Glitch-Exterminator/github-quiz/actions/workflows/ci.yml/badge.svg)](https://github.com/Glitch-Exterminator/github-quiz/actions/workflows/ci.yml)

Консольная викторина по Git и GitHub: пять вопросов по лекции,
ответ — номер варианта, в конце — итог в процентах.

## Как запустить

Нужен .NET 8 или новее.

```bash
git clone https://github.com/<ник>/github-quiz.git
cd github-quiz
dotnet run
```

## Файлы проекта

| Файл | Что внутри |
|------|------------|
| `Program.cs` | задаёт вопросы, проверяет ответы, считает итог |
| `Question.cs` | модель вопроса: текст, варианты, номер правильного |
| `Questions.cs` | список всех вопросов викторины |

> [!TIP]
> Хочешь добавить свой вопрос? Скопируй блок `new(...)` в `Questions.cs`
> и поставь его в конец списка.

## Команда
Изменения в main принимаются только через Pull Request. Как предложить
правку — в [CONTRIBUTING.md](CONTRIBUTING.md).
