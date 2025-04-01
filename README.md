# Домашнее задание к занятию " `Системы контроля версий` " - `Сулименков Алексей`

---

## Задание 1

### Создание репозитория и первого коммита

<details> <summary>git status</summary>

```git
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: README.md

no changes added to commit (use "git add" and/or "git commit -a")
```

</details>

<details> <summary>First commit</summary>

```git
git add . && git commit -am "HW-devops-netology"
[main 1304a10] HW-devops-netology
1 file changed, 25 insertions(+), 1 deletion(-)
```

</details>

---

## Задание 2

### Создание файлов .gitignore и второго коммита

1. Будут игнорироваться файлы содержащие \*.tfvars, \*.tfvars.json, \*\_override.tf, \*\_override.tf.json, \*.tfstate.\*, \*.tfstate, crash.\*.log и т.д.
2. Будут игнорироваться файлы crash.log, override.tf, override.tf.json, .terraformrc, terraform.rc и т.д.
3. Будут игнорироваться папки и все что внутри \*\*/.terraform/\* и tmp\*

<details> <summary>gitignore terraform</summary>

```git
# Local .terraform directories
**/.terraform/*

# .tfstate files
*.tfstate
*.tfstate.*

# Crash log files
crash.log
crash.*.log

# Exclude all .tfvars files, which are likely to contain sensitive data, such as
# password, private keys, and other secrets. These should not be part of version
# control as they are data points which are potentially sensitive and subject
# to change depending on the environment.
*.tfvars
*.tfvars.json

# Ignore override files as they are usually used to override resources locally and so
# are not checked in
override.tf
override.tf.json
*_override.tf
*_override.tf.json

# Ignore transient lock info files created by terraform apply
.terraform.tfstate.lock.info

# Include override files you do wish to add to version control using negated pattern
# !example_override.tf

# Include tfplan files to ignore the plan output of command: terraform plan -out=tfplan
# example: *tfplan*

# Ignore CLI configuration files
.terraformrc
terraform.rc
tmp*
.terraform.lock*
```

 </details>

---

## Задание 3

### Эксперимент с удалением и перемещением файлов (третий и четвёртый коммит)

Добавил нновую строку.
