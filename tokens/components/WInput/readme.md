# Журнал изменений токенов WInput

## Связи переменных

- **style.json** — предоставляет стили и состояния (`label`, `icon`, `contrast`, `soft`) и размеры (`input`, `wrap`).
- **template/WInput.json** — шаблон для состояний и размеров (`sm`, `md`, `lg`, `autoheight`).
- **label/style.json** — отступы для `slot-label` (`gap`, `sp-*`).
- **label/template.json** — шаблон `slot-label` с привязкой к `label/style.json` и `size.wrap`.
- **headlabel/style.json** — типографика (`title-text`, `required-text`, `option-text`) для всех размеров (`sm`, `md`, `lg`, `autoheight`).

## Changelog

1. 28.05.2025 14:00
- Переименованы ключи `placholder` → `placeholder` в `style.json`.
- Исправлены лишние или пропущенные `}` в `style.json` и `label/style.json`.
- Расширены блоки состояний (hover, focus, select, typing, filled, success, error, disable) в `template/WInput.json` для секций `contrast` и `soft`.
- Добавлен раздел `md` в `template/WInput.json`.
- Настроено `autoheight` в `template/WInput.json`: `minHeight` → `{w-input.size.input.sm.height-min}`, `maxHeight` → `{w-input.size.input.lg.height-max}`.
- Добавлены папки `label` и `headlabel` с их `style.json` и `template.json`.
- Создан и заполнен `readme.md` с описанием структуры и связей токенов.

2. 29.05.2025 10:00
- Заменены значения `borderRadius` в секциях `input-headlabel` на `{w-input.size.input.<size>.radius-headlabel}` в `template/WInput.json`.
