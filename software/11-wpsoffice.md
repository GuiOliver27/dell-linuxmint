#Autor: Robson Vaamonde<br>
#Procedimentos em TI: http://procedimentosemti.com.br<br>
#Bora para Prática: http://boraparapratica.com.br<br>
#Robson Vaamonde: http://vaamonde.com.br<br>
#Facebook Procedimentos em TI: https://www.facebook.com/ProcedimentosEmTi<br>
#Facebook Bora para Prática: https://www.facebook.com/BoraParaPratica<br>
#Instagram Procedimentos em TI: https://www.instagram.com/procedimentoem<br>
#YouTUBE Bora Para Prática: https://www.youtube.com/boraparapratica<br>
#Data de criação: 24/07/2022<br>
#Data de atualização: 22/03/2023<br>
#Versão: 0.03<br>
#Testado e homologado no Linux Mint 20.1 Ulyssa, 20.2 Uma e 20.3 Una x64<br>
#Testado e homologado no Linux Mint 21 Vanessa, 21.1 Vera, 21.1 Vera, 21.2 Victoria e 21.3 Virginia x64

#Instalação do WPS Office 2019 + Pacote de Tradução e Dicionário no Linux Mint 20.1 Ulyssa, 20.2 Uma e 20.3 Una x64<br>
#Instalação do WPS Office 2019 + Pacote de Tradução e Dicionário no Linux Mint 21 Vanessa, 21.1 Vera, 21.2 Victoria e 21.3 Virginia x64

[![WPS Office](http://img.youtube.com/vi/PzIgNdJDdFE/0.jpg)](https://www.youtube.com/watch?v=PzIgNdJDdFE "WPS Office")

Link da vídeo aula: https://www.youtube.com/watch?v=PzIgNdJDdFE

Site Oficial do WPS Office: https://www.wps.com/<br>
Novidades da Versão do WPS Office: https://www.wps.com/whatsnew/linux/<br>
AppImage do WPS Office (não oficial): https://apprepo.de/appimage/wps-office<br>
Flatpack (Flathub) WPS Office: https://flathub.org/apps/details/com.wps.Office<br>
Github do Pacote de Tradução: https://github.com/vaamonde/pt_br-wpsoffice

#00_ Verificando as Informações do Sistema Operacional Linux Mint<br>

	Terminal: Ctrl + Alt + T
	
	OBSERVAÇÃO IMPORTANTE: Linux Mint 20.x é derivado do Ubuntu Desktop 20.04.x Focal Fossa 
	OBSERVAÇÃO IMPORTANTE: Linux Mint 21.x é derivado do Ubuntu Desktop 22.04.x Jammy Jellyfish
	sudo cat /etc/os-release
	sudo cat /etc/lsb-release
	sudo localectl

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

#02_ Download do WPS Office 2019 no Linux Mint<br>

	#versão atualizado em: Feb. 21 2024 (11.1.0.11719) 
	#mai informações acesse: https://www.wps.com/pt-BR/whatsnew/linux/
	Site: https://www.wps.com/pt-BR/office/linux/
		Clicar no Pacote: .DEB

#03_ Instalando o WPS Office 2019 no Linux Mint<br>

	01_ Na pasta de Download, clicar duas vezes no Instalador do WPS Office 2019;
		Arquivo: wps-office_*.deb,
	02_ Na tela do Gedbi clicar em: Instalar Pacote;
	03_ Digitar a sua senha e clicar em: <Autenticar>
	03_ Clicar no Menu do Linux Mint, e na busca indexada digitar: WPS Office
	04_ Na tela de: End User License Agreement for WPS Office
		Marcar a opção: Have read and agreed to Kingsoft Office Software e clicar em: <I Confirm>

	#OBSERVAÇÃO IMPORTANTE: Caso apareça a tela de: System Check referente a: Problems below are
	#detected in the system, marque as opções: Do not report again e clique em: <Close>

#04_ Instalando o pacote de Tradução e Dicionário PT-BR do WPS Office 2019 no Linux Mint<br>

	01_ Primeira etapa: Acessar o Terminal
		Atalho: Ctrl + Alt + T

	02_ Segunda etapa.: Instalar o software Git:
		sudo apt update
		sudo apt upgrade
		sudo apt install git vim python2 python3

	03_ Terceira etapa: Clonar o projeto do Github
		git clone https://github.com/vaamonde/pt_br-wpsoffice

	04_ Quarta etapa..: Acessar o repositório clonado localmente
		cd pt_br-wpsoffice/

	05_ Quinta etapa..: Executar o script de atualização do Tradutor e Dicionário
		bash install.sh

	06_ Sexta etapa...: Abrir o WPS Office e verificar se a tradução está funcionando
		Menu
			Pesquisar: WPS

	07_ Sétima etapa..: Procedimentos para corrigir a Falha de Acentuação do WPS Office
		_ Abrir o WPS Office 2019;
		_ na tela inicial do WPS Office clicar em: Global Settings (Definições Globais);
		_ selecionar: settings (Definições);
		_ em Settings Other clicar em: Settings Other Options Popup Component;
		_ alterar para: Multi-Module Mode <OK>;
		_ na tela de Restart WPS to see changes clicar em: <OK>;
		_ Fechar o WPS Office e testar a acentuação no Write e Spreadsheets;
		_ na tela de Verificação do Sistema marque a opção: Não relatar novamente e <Close>