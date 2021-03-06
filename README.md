# Встановлення залежностей

Встановити в проект наступні пакети (після підняття проекту).

```bash
npm install --save-dev prettier husky lint-staged
```

У VSCode додатково встановити плагіни: Prettier, Formatting Toggle та ESLint

## Інтеграція плагінів

Додати у корінь проекту файли із налаштуваннями: .huskyrc, .lintstagedrc та
.prettierrc.json.

Посилання на документацію по інтеграції плагінів в популярні редактори.

- [Prettier editor integration](https://prettier.io/docs/en/editors.html)
- [ESLint editor integration](https://eslint.org/docs/user-guide/integrations)

## Налаштування VSCode

Для комфортної роботи, після встановлення плагінів, потрібно додати налаштування
редактора для форматування файлів.

Зайти у _Settings_, задати пошук _Code Actions On Save_ і у результатах пошуку
натиснути на посилання _Edit in settings.json_. У файлі, що відкриється, вкінці
додати зазначену властивість (або замінити значення, якщо властивість вже
існує):

```json
{
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

[Репозиторій GoIT](https://github.com/goitacademy/react-lint-config)
