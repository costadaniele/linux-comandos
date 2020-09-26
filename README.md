# Comandos Linux

- Para abrir o terminal

`ctrl + alt + t`

- Abrir nova aba

`ctrl + shift + t`

- Limpar a tela

`clear`
`ctrl + l`

- Limpar linha inteira

`ctrl + u`

- Cria diretório

`mkdir`

- Cria um arquivo em branco 

`touch`

- Move um arquivo ou pasta 

`mv`

- Copia um arquivo ou pasta

`cp`

- Troca de diretório.

- `cd` 

- Lista o conteúdo do diretório atual.

- `ls` 

- Para ver o diretório atual.

- `pwd` 

- Diretório atual.

- `.` 

- Diretório anterior.

- `..` 

- Manual - Ex. man ls

- `man`

   - NAME: nome completo do comando.
   - SYNOPSIS: Mostra que argumentos o comando leva.
   - DESCRIPTION: Explica de forma mais completa o NAME e a SYNOPSIS.

- Remover

- `rm`

- Saber o usuário

`whoami`

- Logout

`ctrl + d` ou `exit` ou `logout`

---

- Tipos de gerenciadores de pacotes

`apt`, `dpkg`, `pip`, `npm`

--- 

- Exemplo de biblioteca python - numpy - para usar a matemática

`pip install numpy`

---

### GUI:

Graphical User Interface.

- Interface

### CLI

Command Line Interface. 

- Interface não gráfica.

--- 

## Hierarquia no Linux

- Arquivos organizados em árvore

- `/` - diretório raiz

- `~` - home

---

## Caminho relativo e caminho absoluto

- Caminho relativo `./`

   - `cd Dowloads/`
   - o Linux entende que você colocou o ./ para o diretório atual.

- Caminho absoluto - começa com `/`

   - `cd /home/dani/Downloads/`

---

## Passando argumentos para os comandos

- Forma abreviada

   - `ls -a` - all, todos os arquivos listados.

- Forma completa

   - `ls --all`

- Listando os diretórios no formato longo.

   - `ls -l`

- Forma combinada, listada com arquivos ocultos

   - `ls -la`

- Manual do manual

   - `man man`

--- 

## Gerenciamento de software

- Gerenciadores de pacotes
  
   - dpkg, arquivo local
   - instala arquivos .deb `sudo dpkg -i nomedopacote.deb`
   - r (remover) `sudo dpkg -r nomedoprograma`
   - retira o arquivo do sistema `sudo dpkg --purge nomedoprograma`
   - i (install)
   - `sudo dpkg -l` lista os pacotes instalados por dpkg
   - `dpkg -l | grep nomedoprograma` para achar programa

---

   - apt (busca o pacote nos respositórios oficias do seu linux.)
   - procura na internet e procura o arquivo.
   - `sudo apt install nomedoprograma`
   - `sudo apt update` atualiza as informações de software.
   - `sudo apt upgrade` atualiza todos os software.
   - `sudo apt update && sudo apr upgrade`

   - sudo (permissão de super usuário) `sudo apt install cowsay`


## Extras

- Programas
   - `sudo apt install cowsay`
   - `sudo apt install xcowsay`
   - `sudo apt install cmatrix`


- editar no terminal `nano /etc/apt/sources.list` repositórios oficiais

- Ver dependências
   - `apt-cache search nomedoprograma`
   - `apt-cache show nomedoprograma`

- Problemas de dependências
   - `sudo apt install -f`

---

instalação open source `sudo apt install nomedoprograma`

- software proprietário 

   -`.deb`
   - instalar repositório
   - snap store


--- 

`sudo apt install snapd`
`sudo snap install snap-store`


---

Editar texto no terminal

- `nano texto.txt`
- `control + x` - sair
- `y` - salvar

   - `^` - control
   - `m` - alt
   - `ctrl + g` - ajuda
   - `ctrl + o` - salvar

---

Editores

- nano

- vim
   - `sudo apt install vim`
   - `vimtotur`
   - `:q` - para sair
   - `:q!` - sair e salvar

- emacs

---

- Usuários, grupos, permissões

`cat /etc/passwd`
`cat /etc/group`

- Filtra o conteúdo

`grep nomedogrupo /etc/passwd`


---

Calendário

`cal`
`cal 06 2020`
`cal 2020`

---

Data

`date`

---

Imprimir - com impressora conectada

`lpr`

---

Informações do usuário

`finger`

---

Repete o último comando

- `sudo !!`

---

- Adicionar usuário

`adduser nome`

- Mudar usuário

`su - dani`

- Superusuário

`sudo su`

- Deletar usuário

`sudo userdel dani`

- Listar UID, GID e grupos

`id`

- Deletar usuário

`sudo userdel dani`

- Deletar usuário de um grupo

`sudo deluser dani`

- Adiciona usuário em um grupo.

`usermod -aG sudo dani`

- traceroute é uma ferramenta de diagnóstico que rastreia a rota de um pacote através de uma rede de computadores que utiliza os protocolos IP e o ICMP, implementada pela primeira vez por Van Jacobson em 1988. Atualmente está disponível em diversos sistemas operacionais como Linux, FreeBSD, NetBSD, MacOS X e Windows.

`traceroute`



Referência:

Curso de Terminal Linux - Daniel Berg

https://www.youtube.com/playlist?list=PLbV6TI03ZWYXXwbP2TNTbviUaFh6YqqVt

---

