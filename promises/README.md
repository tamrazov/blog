# Что такое промисы? и как они работают?

## Уровень первый

Промисы - это объект, который дает возможность для совершения отложенных и асихронных вычислений.

Состояния:
- pending — стартовое состояние, операция стартовала
- fulfilled — получен результат
- rejected — ошибка

```js
const promise = new Promise()

promise
  .then(() => {
    console.log('Код выполняется в случае успеха')
  })
  .catch(() => {
    console.log('Код выполнится в случае неуспеха')
  })
```