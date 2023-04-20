# Личный проект «Gllacy»

* Студент: [Илья Жилин](https://htmlacademy.ru/profile/id535607).
* Наставник: [Артур Трифонов](https://htmlacademy.ru/profile/wrgraff).


---

_Не удаляйте файлы настроек проекта:_

* `.editorconfig`,
* `.gitattributes`,
* `.gitignore`,
* `.stylelintrc`,
* `gulpfile.js`,
* `package-lock.json`,
* `package.json`,
* `Contributing.md`,
* `Readme.md`.

---

## Установка зависимостей проекта

В локальном репозитории уже можно писать разметку страниц, стили и создавать прочие файлы. Но разрабатывать проект будет удобнее с дополнительными инструментами (зависимостями). А для этого их установить.

### 1. Терминал

Для установки зависимостей понадобится терминал. В Linux и macOS он уже есть, а в Windows лучше установить _git-bash_, который идёт в комплекте с самим [Git](https://git-scm.com/download/windows).

### 2. Node.js

Зависимости работают в среде _node.js_, которую тоже нужно установить, но лучше не с помощью установщика с официального сайта, а через менеджер версий ноды. Есть разные менеджеры, но проще всего установить и использовать [_volta_](https://volta.sh/).

Для установки _volta_ в Linux и macOS в терминале выполни:

```shell
curl https://get.volta.sh | bash
```

В Windows проще скачать и запустить [установщик](https://github.com/volta-cli/volta/releases/download/v1.1.1/volta-1.1.1-windows-x86_64.msi).

После установки _volta_ перезапусти (или просто открой новый) терминал и выполни установку _node.js_ свежей LTS версии:

```shell
volta install node
```

После этого выполни:

```shell
node -v
```

Команда должна выдать версию ноды (например `18.16.0`), что означает успешность установки.

### 3. Зависимости

Вместе с нодой стал доступен её менеджер пакетов — _npm_. Можно было бы использовать его, но лучше воспользоваться его альтернативой — _pnpm_. Установи его через _volta_:

```shell
volta install pnpm
```

> В Windows эта команда может завершиться с ошибкой (_pnpm_ не установится). В таком случае в настройках системы нужно включить режим «Для разработчика» (официальная [инструкция](https://learn.microsoft.com/ru-ru/windows/apps/get-started/enable-your-device-for-development#accessing-settings-for-developers)), перезагрузиться и заново запустить команду.

После этого для установки зависимостей проекта в терминале, находясь в директории проекта, выполни:

```shell
pnpm i
```

> **Не** обращай внимание на предупреждения во время установки.

После установки зависимостей можно запускать линтинг:

```shell
pnpm run lint
```

И сборку для разработки:

```shell
pnpm run start
```

При этом запустится и локальный сервер, а в брауезере откроется разрабатываемый сайт и будет обновляться при обновлении файлов в проекте.

> Кстати, в этих командах можно уже использовать _npm_ вместо _pnpm_. Они будут так же работать.

---

<a href="https://htmlacademy.ru/intensive/htmlcss"><img align="left" width="50" height="50" alt="HTML Academy" src="https://up.htmlacademy.ru/static/img/intensive/htmlcss/logo-for-github-2.png"></a>

Репозиторий создан для обучения на профессиональном онлайн‑курсе «[HTML и CSS. Профессиональная вёрстка сайтов](https://htmlacademy.ru/intensive/htmlcss)» от [HTML Academy](https://htmlacademy.ru).

[check-image]: https://github.com/htmlacademy-htmlcss/000000000000000-sedona-37/workflows/Project%20check/badge.svg?branch=master
[check-url]: https://github.com/htmlacademy-htmlcss/000000000000000-sedona-37/actions
