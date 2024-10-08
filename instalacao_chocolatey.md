# Script de Instalação de Ferramentas de Desenvolvimento com Chocolatey

Este script utiliza o **Chocolatey** para instalar todas as ferramentas necessárias para o ambiente de desenvolvimento.

## Atualiza Chocolatey
```
choco upgrade chocolatey
```

## Instalação das Ferramentas

Abaixo estão as ferramentas que serão instaladas. Você pode adicionar ou remover conforme suas necessidades:

```powershell
# Instalação das ferramentas
choco install git -y
choco install nodejs -y
choco install vscode -y
choco install docker-desktop -y
choco install googlechrome -y
choco install postman -y
choco install java.jdk -y
choco install intellijidea-community -y
```

## Como Usar

1. Copie o conteúdo deste script.
2. Abra o **PowerShell** como administrador.
3. Cole o script no terminal e pressione **Enter**.
4. O script irá instalar as ferramentas listadas.