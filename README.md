# SysmoUpdater-SysmoS1-Guia
Guias, manuais, dicas, este repositório será exclusivo para compartilhar informações sobre a atualização do SysmoS1 utilizando o SysmoUpdater

---


### Instaladores disponíveis nas versões:
- [Windows](https://www.sysmo.com.br/sysmo03/sysmo-updater-s1/instalador/windows/Instalador-SysmoUpdater-SysmoS1.exe)
- [Linux](https://www.sysmo.com.br/sysmo03/sysmo-updater-s1/instalador/linux/instalarSysmoUpdater.zip) ou `wget -c https://www.sysmo.com.br/sysmo03/sysmo-updater-s1/instalador/linux/instalarSysmoUpdater.zip`

---


### Demonstração:
[![guia-instalacao-image]][guia-instalacao-video]

---


### Manual:
- [Instalação Servidor][instalacao-servidor]
- [Instalação Estações (Apenas Windows)][instalacao-estacao]



---


### SysmoUpdater - Pagina web
**Acesso:**
- http://**\< IP do Servidor \>**:5555/sysmo-updater-api/api/ 
- Usuário: `sysmo`
- Senha: `updater36310600`

---


### SysmoUpdater - Projetos
**Projetos utilizados no processo de atualização:**
- ![acesso-projetos-1]

---


### SysmoUpdater - Estações
**Cadastro de Estações:**
- Nesta tela devem ser cadastrados os terminais, mapeando sempre pelo endereço de IP, e utilizando a porta 5555.
![acesso-estacoes-1]

---


### SysmoUpdater - Agendamentos
![acesso-agendamentos-1]

**Preparar os arquivos e disponibilizar para as estações:**
- Preparar os arquivos e disponibilizar para as estações.
Neste passo devem ser adicionados os arquivos do build na pasta `c:\sysmo-updater\upload\pacote` ou `/usr/lib/sysmo-updater/upload/pacote/`
![acesso-agendamentos-2]

- No campo tipo de execução, deve-se escolher o tipo de execução, se será executado imediatamente ou via agendamento.

- Adicionar o projeto.
![acesso-agendamentos-3]

- Cadastrar os terminais.
![acesso-agendamentos-4]

- E conferir se o script está correto.
![acesso-agendamentos-5]

- Serão transferidos para o terminal somente os arquivos da versão necessários.

**Fechar os programas abertos e bloquear as conexões com a base.**
- Lembrando que para os processos a seguir funcionarem corretamente, o terminal deverá estar com o dbxconnections direcionado para a máquina que é o Servidor de dados. Por isso a necessidade do sysmo-updater estar instalado no mesmo servidor de dados.
![acesso-agendamentos-6]

- Os arquivos ficarão salvos na pasta `c:\sysmo-updater\upload\estacoes\arquivosAtualizacao`, nos terminais.
![acesso-agendamentos-7]

**Atualização da base de dados e disponibilização dos binários atualizados**
- Lembrando que como o sistema faz o processo de atualização, não é necessário rodar o Atlsysmo no servidor de dados.
![acesso-agendamentos-8]

**Reabrir os programas e liberar as conexões do banco de dados**
- Nos terminais, este processo vai abrir os programas que estavam abertos, e reestabelecer a conexão com o banco de dados que foi bloqueado nos agendamentos anteriores
![acesso-agendamentos-9]

**Utilitarios - Disponibilizar executáveis especificos para as estações**
- Disponível para atualização de executáveis específicos de versões, como por exemplo, 2.24.04.006a
![acesso-agendamentos-10]
![acesso-agendamentos-11]

---


[//]: # (Links:)
[instalacao-servidor]: ./manual/instalacao/servidor.md
[instalacao-estacao]: ./manual/instalacao/estacao.md


[//]: # (Links relacionado ao video)
[guia-instalacao-image]: ./images/video-play.jpeg
[guia-instalacao-video]: https://drive.google.com/file/d/1EqF_IuVJkX67Xy7sJ9Hsr4_QSLaenap4/view


[//]: # (Links relacionado a aba Projetos do SysmoUpdater)
[acesso-projetos-1]: ./images/acesso-projetos-1.jpeg

[//]: # (Links relacionado a aba Estações do SysmoUpdater)
[acesso-estacoes-1]: ./images/acesso-estacoes-1.jpeg


[//]: # (Links relacionado a aba Agendamentos do SysmoUpdater)

[//]: # (Links relacionado ao Primero passo do projeto)
[acesso-agendamentos-1]: ./images/acesso-agendamentos-1.jpeg
[acesso-agendamentos-2]: ./images/acesso-agendamentos-2.jpeg
[acesso-agendamentos-3]: ./images/acesso-agendamentos-3.jpeg
[acesso-agendamentos-4]: ./images/acesso-agendamentos-4.jpeg
[acesso-agendamentos-5]: ./images/acesso-agendamentos-5.jpeg

[//]: # (Links relacionado ao Segundo passo do projeto)
[acesso-agendamentos-6]: ./images/acesso-agendamentos-6.jpeg
[acesso-agendamentos-7]: ./images/acesso-agendamentos-7.jpeg

[//]: # (Links relacionado ao Terceiro passo do projeto)
[acesso-agendamentos-8]: ./images/acesso-agendamentos-8.jpeg

[//]: # (Links relacionado ao Quarto passo do projeto)
[acesso-agendamentos-9]: ./images/acesso-agendamentos-9.jpeg

[//]: # (Links relacionado ao Quinto passo do projeto)
[acesso-agendamentos-10]: ./images/acesso-agendamentos-10.jpeg
[acesso-agendamentos-11]: ./images/acesso-agendamentos-11.jpeg

