# gh-actions-setup-ssh
Action для GitHub Actions по настройке SSH сессии

Пример использования:

```
jobs:
  ...
    steps:
      - uses: tutu-ru-mobile/gh-actions-setup-ssh@v1
        with:
          ssh-private-key: "${{ secrets.SSH_PRIVATE }}"
      - run: # Тут уже работает под нашим ssh ключом (git push и всё такое)

```
