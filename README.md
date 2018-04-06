# Домашнее задание "Типизация"

Домашнее задание #9 в ШРИ Яндекса 2018.

## Задание

Необходимо типизировать функцию [extend](https://gist.github.com/alt-j/9dae0e73b118370cf54f2d08a22e02de) с помощью двух инструментов:

- [x] TypeScript
- [ ] Flow

Задача написать максимально надежный (type safety) код.

Результатом задания должны быть две ссылки, содержащие переписанный код, на:

- [typescriptlang.org/play](https://www.typescriptlang.org/play)
- [flow.org/try](https://flow.org/try)

## Выполнение задания

- Настроил инфраструктуру для работы с TypeScript и Flow.
- Написал тесты, для того, чтобы проверить функциональность данной функции на TypeScript-е и Flow.

### TypeScript

- Выделил интерфейс `IObject` для определения типов объектов с перечисляемыми свойствами.
- Разбил аргументы функции `extend` на две части: `head` и `tail`, для того что бы тип `boolean` был разрешен только для первого аргумента.
- Так и не понял как исключить `null` из типа `IObject`, ибо в случае передачи его в качестве первого аргумента, будет ошибка.
