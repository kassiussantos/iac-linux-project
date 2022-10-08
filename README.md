# Atividade Bootcamp dio.me

Cloud DevOps Experience - Banco Carrefour

Script de Criação de Estrutura de Usuários, Diretórios e Permissões

## **Descrição**

Neste projeto iremos criar um script onde toda a infraestrutura de usuários, grupos de usuários, diretórios e permissões serão criadas automaticamente. Será realizado o upload do arquivo de script no GitHub para futuras reutilizações do script. Sendo assim, toda nova máquina virtual que for iniciada já estará pronta para uso quando o script for executado.

### Pré-requisitos:

- Linux, Git e GitHub

## Extras

_Obs:  Abaixo um script rapido com "for in" para remover os usuários e grupos criados durante as aulas de Linux no Bootcamp. O nome do meu arquivo é **`create_user.sh`** é só trocar para o nome do arquivo que vocês criaram._

- ==> Para remover os Usuarios <==

```bash
for i in $(cat create_user.sh |grep useradd |cut -d" " -f2); do userdel -r -f $i; done
```
- ==> Para remover os grupos <==

```bash
for i in $(cat create_user.sh |grep groupadd |cut -d" " -f2); do groupdel $i; done
```

