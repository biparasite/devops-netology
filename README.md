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

<details> <summary>git log</summary>
```git
commit 1dc077e6e35e13325927e3c4177328c7a4cd7374 (HEAD -> main, origin/main, origin/HEAD)
Author: biparasite <biparasite@gmail.com>
Date:   Sat Mar 29 13:59:15 2025 +0300

    Moved and deleted

commit 7db205c96061a00a2d6680df9f6437471b0f7480
Author: biparasite <biparasite@gmail.com>
Date: Sat Mar 29 13:55:44 2025 +0300

    Prepare to delete and move

commit 171b5528d98cb8a988ba63f5cc051ed49d441375
Author: biparasite <biparasite@gmail.com>
Date: Sat Mar 29 13:52:30 2025 +0300

    gitignore

commit 6ab32165ad299fae59259dec04615400360ff8f6
Author: biparasite <biparasite@gmail.com>
Date: Sat Mar 29 13:17:32 2025 +0300

    HW-devops-netology

commit 733b13131cca34f2d2b1151aa14aca762d20c508
Author: biparasite <biparasite@gmail.com>
Date: Sat Mar 29 13:15:45 2025 +0300

    HW-devops-netology

commit 1304a10c2f701fab38eeeb0e00cd59207b986a9b
Author: biparasite <biparasite@gmail.com>
Date: Sat Mar 29 13:13:06 2025 +0300

    HW-devops-netology

commit a45c848e513f41fab63a0a834c40dc4e299e0040
Author: biparasite <117280737+biparasite@users.noreply.github.com>
Date: Sat Mar 29 12:51:31 2025 +0300

    Initial commit

```

 </details>
```
