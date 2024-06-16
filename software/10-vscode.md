#Autor: Robson Vaamonde<br>
#Procedimentos em TI: http://procedimentosemti.com.br<br>
#Bora para Prática: http://boraparapratica.com.br<br>
#Robson Vaamonde: http://vaamonde.com.br<br>
#Facebook Procedimentos em TI: https://www.facebook.com/ProcedimentosEmTi<br>
#Facebook Bora para Prática: https://www.facebook.com/BoraParaPratica<br>
#Instagram Procedimentos em TI: https://www.instagram.com/procedimentoem<br>
#YouTUBE Bora Para Prática: https://www.youtube.com/boraparapratica<br>
#Data de criação: 31/05/2022<br>
#Data de atualização: 22/03/2024<br>
#Versão: 0.05<br>
#Testado e homologado no Linux Mint 20 Ulyana, 20.1 Ulyssa, 20.2 Uma e 20.3 Una x64<br>
#Testado e homologado no Linux Mint 21 Vanessa, 21.1 Vera, 21.2 Victoria e 21.3 Virginia x64

#Instalação do Microsoft Visual Studio Code VSCode no Linux Mint 20 Ulyana, 20.1 Ulyssa, 20.2 Uma e 20.3 Una x64<br>
#Instalação do Microsoft Visual Studio Code VSCode no Linux Mint 21 Vanessa, 21.1 Vera, 21.2 Victoria e 21.3 Virginia x64

[![VSCode](http://img.youtube.com/vi/faS3gZgKE-A/0.jpg)](https://www.youtube.com/watch?v=faS3gZgKE-A "VSCode")

Link da vídeo aula: https://www.youtube.com/watch?v=faS3gZgKE-A

Site Oficial do Visual Studio Code: https://code.visualstudio.com/<br>
Site Oficial do Visual Studio Code Web: https://vscode.dev/<br>
Link do Marketplace: https://marketplace.visualstudio.com/VSCode

O QUE É E PARA QUE SERVER O VSCODE: O Visual Studio Code é um editor de código-fonte desenvolvido<br>
pela Microsoft para Windows, Linux e macOS. Ele inclui suporte para depuração, controle de<br> 
versionamento Git incorporado, realce de sintaxe, complementação inteligente de código, snippets e<br> 
refatoração de código.

#00_ Verificando as Informações do Sistema Operacional Linux Mint<br>

	Terminal: Ctrl + Alt + T

	#OBSERVAÇÃO IMPORTANTE: Linux Mint 20.x é derivado do Ubuntu Desktop 20.04.x Focal Fossa 
	#OBSERVAÇÃO IMPORTANTE: Linux Mint 21.x é derivado do Ubuntu Desktop 22.04.x Jammy Jellyfish
	sudo cat /etc/os-release
	sudo cat /etc/lsb-release

	Menu
		Informações do Sistema
		
#01_ Atualização do Sistema Operacional Linux Mint<br>

	_ Atualização do sistema utilizando o MintUpdate;
	_ Atualização do sistema utilizando o Apt;

	Terminal: Ctrl + Alt + T
		sudo apt update
		sudo apt upgrade
		sudo apt full-upgrade
		sudo apt dist-upgrade
		sudo apt autoremove
		sudo apt autoclean

#02_ Instalando as Dependências do Microsoft Visual Studio Code VSCode no Linux Mint<br>

	#instalando as dependências do VSCode
	sudo apt install vim git python2 python3 cloc

#03_ Baixando o Microsoft Visual Studio Code VSCode para o Linux Mint<br>

	https://code.visualstudio.com/download
		Versão: .deb (Debian, Ubuntu 64 Bits)
			Salvar aquivo

#04_ Instalando o Microsoft Visual Studio Code VSCode utilizando o Gdebi-Gtk no Linux Mint<br>

	Arquivos
		Download
			code_1.*_amd64
				Instalar Pacote
			Fechar

#05_ Verificando o novo repositório do Microsoft Visual Studio Code VSCode no MintUpdate<br>

	Menu
		MintUpdate
			Editar
				Fontes de Programas
					(Digite a senha do seu usuário)
						Repositórios Adicionais
							Habilitado: Microsoft / Stable - code
						Chaves de Autenticação
							Microsoft (Release signing)
				Fechar
		Fechar

#06_ Iniciando o Microsoft Visual Studio Code VSCode no Linux Mint<br>

	Menu
		Busca Indexada
			vscode
				Dark Theme
				Notifications: Pacote PT-BR
				Disable: Mostrar página inicial na inicialização

#07_ Configurando o Microsoft Visual Studio Code VSCode como Aplicativo de Preferência no Linux Mint<br>

	Menu
		Busca Indexada
			Aplicativos de Preferencias
				Texto puro: Visual Studio Code
				Código fonte: Visual Studio Code

#08_ Instalando e Configurando as Principais Extensões Microsoft Visual Studio Code VSCode<br>

	Portuguese (Brazil) Language Pack for Visual Studio Code
		(Sem necessidade de configuração)

	Brazilian Portuguese - Code Spell Checker (Corretor Ortográfico de Código)
	Manter selecionado a extensão: Brazilian Portuguese - Code Spell Checker
		Pressionar F1
			Show Spell Checker Configuration Info
				User
					Language
						English (en_us)
						Portuguese (pt_br)
						Portuguese - Brazil (pt-br)
					File Types and Programming Languages
						shellscript, python, markdown, etc...

	Code Spell Checker
		(Sem necessidade de configuração)

	Bats (Bash Automated Testing System)
		(Sem necessidade de configuração)

	Bash Beautify
		(Sem necessidade de configuração)

	Shell-Format
		(Sem necessidade de configuração)

	ShellCheck
		(Sem necessidade de configuração)

	Cisco IOS Syntax
		(Sem necessidade de configuração)

	Cisco IOS-XR Syntax
		(Sem necessidade de configuração)

	Cisco Config Highlight
		(Sem necessidade de configuração)

	Pylance
		(Sem necessidade de configuração)

	Python
		(Sem necessidade de configuração)

	Docker
		(Sem necessidade de configuração)

	Powershell
		(Sem necessidade de configuração)

	Ansible
		(Sem necessidade de configuração)

	YAML
		(Sem necessidade de configuração)

	MySQL
		(Sem necessidade de configuração)

	Remote - SSH
		(Sem necessidade de configuração)

	NoSQL
		(Sem necessidade de configuração)

#09_ Configurações básicas do Microsoft Visual Studio Code VSCode para funcionar perfeitamente no Linux Mint<br>

	Gerenciar
		Configurações
			Code Spell Checker
				C Spell: Enabled Language Ids: 
					Adicionar Item: shellscript
				C Spell: Language: en,pt,pt-BR
				C Spell: Max Duplicate Problems: 500000
				C Spell: Max Number Of Problems: 500000
			Editor
				Editor: Tab Size: 4
				Editor: Detect Indentation: False (Off)
				Editor: Insert Spaces: False (Off)
				Render Whitespace: All
			Files
				Files: Eol: \n (LF)

			#OBSERVAÇÃO IMPORTANTE: executar essa configuração somente se você fez a instalação
			#do ZSH, das Fontes Hack e do Oh My ZSH.
			Font
				Integrated: Font Family
					Hack Nerd Font
			
			#Configuração do Terminal Padrão do VSCODE
			Ctrl + Shift + P
				Terminal: Selecionar o Perfil Padrão
					zsh