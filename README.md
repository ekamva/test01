# Команды git pull и git fetch
## 1. Что делают команды:

**git fetch**: Загружает последние изменения (коммиты, ветки, теги и т.д.) с удалённого репозитория в ваш локальный репозиторий, но не объединяет эти изменения с вашей текущей веткой. После выполнения этой команды вы видите, какие изменения были внесены в удалённый репозиторий, и можете вручную решить, как их интегрировать (например, с помощью *git merge* или *git rebase*).

`**git pull**`: Делает то же самое, что и *git fetch*, но с последующим автоматическим объединением (merge) загруженных изменений с вашей текущей веткой. Эта команда является комбинацией *git fetch* и *git merge* в одном шаге.

## 2. Когда использовать:

**git fetch**: Используйте, когда вы хотите увидеть изменения в удалённом репозитории перед их интеграцией в свою ветку. Это позволяет просмотреть изменения и избежать автоматического мерджа, что может быть полезно для предотвращения неожиданных конфликтов.

**git pull**: Используйте, когда вы уверены, что хотите получить и сразу объединить изменения с удалённого репозитория с вашей текущей веткой. Это удобно, когда вы хотите быстро синхронизироваться с удалённой веткой.

## 3. Риски:

**git fetch**: Безопасен в использовании, поскольку он просто загружает данные и не меняет вашу текущую ветку. Это позволяет вам контролировать процесс слияния и избежать конфликтов, которые могут возникнуть при автоматическом слиянии.

**git pull**: Может привести к неожиданным конфликтам, если удалённые изменения конфликтуют с вашими локальными. В этом случае вам придётся разрешать конфликты вручную.

## 5. Выводы

Таким образом, **git fetch** предоставляет больше контроля, позволяя сначала просмотреть изменения, в то время как **git pull** является более автоматизированным и быстрым способом синхронизации с удалённой веткой, но с определёнными рисками.


