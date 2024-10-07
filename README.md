
# Meu Repositório de Dotfiles

Este repositório contém minhas configurações pessoais (**dotfiles**) para diversos programas e ferramentas que utilizo no meu ambiente de desenvolvimento. Com ele, posso replicar facilmente minhas configurações em qualquer máquina.

## Arquivos Incluídos

- **.gitconfig**: Configurações globais para o Git, incluindo nome de usuário, e-mail e preferências de merge.
- **.lesshst**: Histórico de navegação do `less`, um pager de arquivos de texto.
- **.docker**: Configurações do Docker para facilitar o uso e personalização.

## Como Usar

### Clonar o Repositório

Para usar esses **dotfiles** em outro sistema, siga os passos abaixo:

1. Clone o repositório para o seu diretório home:

   ```bash
   git clone https://github.com/SEU_USUARIO/dotfiles.git ~/dotfiles
   ```

2. Navegue até o diretório dos **dotfiles**:

   ```bash
   cd ~/dotfiles
   ```

3. Crie os **symlinks** para os arquivos no diretório home:

   #### No Linux/macOS:
   ```bash
   ln -s ~/dotfiles/.gitconfig ~/.gitconfig
   ln -s ~/dotfiles/.lesshst ~/.lesshst
   ln -s ~/dotfiles/.docker ~/.docker
   ```

   #### No Windows (usando Prompt de Comando):
   ```cmd
   mklink C:\Users\seu_usuario\.gitconfig C:\Users\seu_usuario\dotfiles\.gitconfig
   mklink C:\Users\seu_usuario\.lesshst C:\Users\seu_usuario\dotfiles\.lesshst
   mklink /D C:\Users\seu_usuario\.docker C:\Users\seu_usuario\dotfiles\.docker
   ```

### Atualizar os Dotfiles

Sempre que alterar alguma configuração, você pode atualizar o repositório seguindo os passos:

1. Faça suas alterações nos arquivos de configuração.
2. Adicione as alterações ao Git:

   ```bash
   git add .
   ```

3. Faça o commit das alterações:

   ```bash
   git commit -m "Atualização das configurações"
   ```

4. Envie as alterações para o GitHub:

   ```bash
   git push origin master
   ```

## Estrutura do Repositório

A estrutura do repositório é a seguinte:

```
dotfiles/
├── .gitconfig
├── .lesshst
└── .docker/
```
