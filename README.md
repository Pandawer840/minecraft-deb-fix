# ⛏️ Minecraft Launcher — Debian Dependency Fix

Uma versão corrigida do instalador `.deb` oficial do **Minecraft: Java Edition** para distribuições baseadas em Debian.

> ⚠️ **Este projeto não é afiliado, mantido ou endossado pela Mojang Studios ou Microsoft.**

---

## 🐛 O Problema

O pacote `.deb` original distribuído pela **Mojang/Microsoft** até o momento(25-09-2026), contém um erro na nomenclatura de uma de suas dependências: **falta um hífen (`-`)** no nome do pacote.

Esse erro pode impedir a instalação automática através do `dpkg` ou `apt` em distribuições como:

* Debian
* Ubuntu
* Linux Mint
* Pop!_OS
* Outras distribuições derivadas

---

## 🛠️ A Solução

O pacote `.deb` oficial foi:

1. 📦 Descompactado;
2. 🔧 Corrigido no arquivo de metadados `control`;
3. 📦 Reempacotado novamente no formato `.deb`.

### 🔒 Integridade do conteúdo

**Nenhuma alteração foi feita nos arquivos executáveis ou binários internos do jogo.**

A correção é **exclusivamente relacionada à estrutura e às dependências do pacote Debian**.

---

## 🚀 Como Baixar e Instalar

### 1. Baixe o pacote

Acesse a seção **[Releases](../../releases)** deste repositório e baixe o arquivo:

```text
Minecraft-Fixed.deb
```

### 2. Abra o terminal

Navegue até a pasta onde o arquivo `.deb` foi baixado.

Por exemplo:

```bash
cd ~/Downloads
```

### 3. Instale o pacote

Execute:

```bash
sudo dpkg -i Minecraft-Fixed.deb
```

Caso existam dependências pendentes, execute:

```bash
sudo apt-get install -f
```

---

## 📋 Compatibilidade

Este pacote foi desenvolvido para distribuições que utilizam o sistema de empacotamento **Debian (`.deb`)**, incluindo:

| Distribuição               | Compatibilidade |
| -------------------------- | --------------- |
| Debian                     | ✅               |
| Ubuntu                     | ✅               |
| Linux Mint                 | ✅               |
| Pop!_OS                    | ✅               |
| Derivadas do Debian/Ubuntu | ✅               |

> * A compatibilidade pode variar de acordo com a versão da distribuição e suas dependências disponíveis.

---

## ⚠️ Aviso Legal

Este projeto:

* ❌ **Não é afiliado à Mojang Studios.**
* ❌ **Não é afiliado à Microsoft.**
* ❌ **Não é mantido ou endossado por nenhuma dessas empresas.**
* ❌ **Não contém uma cópia modificada do jogo.**
* ❌ **Não fornece versões piratas do Minecraft.**

O objetivo deste repositório é **exclusivamente corrigir um problema de compatibilidade na estrutura do pacote `.deb` oficial**.

O usuário deve obter o Minecraft e possuir uma licença válida para utilizá-lo.

---

## 📜 Licença

Este repositório contém apenas a correção estrutural necessária para o empacotamento Debian.

Os direitos autorais e demais direitos relacionados ao **Minecraft: Java Edition** permanecem pertencentes aos seus respectivos detentores.

---

<div align="center">

**⛏️ Minecraft Launcher — Debian Dependency Fix**

*Uma pequena correção para um grande problema de empacotamento.*

</div>
