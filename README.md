# AJS-10.3

# Домашнее задание к лекции «Promises, async/await»

**Важно**: каждая задача выполняется в виде отдельного проекта с собственным GitHub репозиторием.

**Важно**: код должен проходить ESLint без ошибок.

**Важно**: тесты должны обеспечивать 100% покрытие тестируемых функций по строкам.

**Важно**: решения должны быть построены на базе [шаблона Webpack](/ci-template).

В личном кабинете на сайте [netology.ru](http://netology.ru/) в поле комментария к домашней работе вставьте ссылки на ваш GitHub-проекты.

---

## Testing Async code (задача со звёздочкой)

**Важно**: данная задача не является обязательной 

### Легенда

Асинхронный код - это здорово, но заглушки, которые были в предыдущих задачах всегда resolv'ятся, а в реальной жизни так бывает не всегда.

### Описание

Используя механизмы Jest, замокайте функции-заглушку `read`, чтобы у вас была возможность протестировать как `resolve`, так и `reject` на выходе из этой функции.

Должно обеспечиваться 100% покрытие функций и классов, которые вы тестируете. Обратите внимание, что вы тестируете асинхронный код.

**Подсказка**: чтобы было удобно замокать эту функцию, вынесите её в отдельный модуль.

Не забудьте написать unit-тесты, которые обеспечивают 100% покрытие функций и классов, которые вы тестируете. Обратите внимание, что вы тестируете асинхронный код.

Обратите внимание, для упрощения настройки Babel лучше добавить отдельную конфигурацию для режима тестирования (в файле `.babelrc`) после `presets` добавьте:

```json
  "env": {
    "test": {
      "presets": [
        [
          "@babel/preset-env",
          {
            "targets": {
              "node": "current"
            }
          }
        ]
      ]
    }
  }
```

### Mock's

[![Build status](https://ci.appveyor.com/api/projects/status/tux5wpe2it4e0r0l/branch/main?svg=true)](https://ci.appveyor.com/project/222Alexa44925/ajs-10-3/branch/main)

---