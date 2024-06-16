#Autor: Robson Vaamonde<br>
#Procedimentos em TI: http://procedimentosemti.com.br<br>
#Bora para Prática: http://boraparapratica.com.br<br>
#Robson Vaamonde: http://vaamonde.com.br<br>
#Facebook Procedimentos em TI: https://www.facebook.com/ProcedimentosEmTi<br>
#Facebook Bora para Prática: https://www.facebook.com/BoraParaPratica<br>
#Instagram Procedimentos em TI: https://www.instagram.com/procedimentoem<br>
#YouTUBE Bora Para Prática: https://www.youtube.com/boraparapratica<br>
#Data de criação: 15/08/2022<br>
#Data de atualização: 12/11/2023<br>
#Versão: 0.07<br>
#Testado e homologado no Linux Mint 20.1 Ulyssa, 20.2 Uma e 20.3 Una x64<br>
#Testado e homologado no Linux Mint 21 Vanessa, 21.1 Vera, 21.1 Vera, 21.2 Victoria e 21.3 Virginia x644

#Instalação do Arduino IDE 2.x no Linux Mint 20.1 Ulyssa, 20.2 Uma e 20.3 Una x64<br>
#Instalação do Arduino IDE 2.x no Linux Mint 21 Vanessa, 21.1 Vera, 21.1 Vera, 21.2 Victoria e 21.3 Virginia x64

[![Arduino 2.x](http://img.youtube.com/vi/ByK8ADwI2mY/0.jpg)](https://www.youtube.com/watch?v=ByK8ADwI2mY "Arduino 2.x")

Link da vídeo aula: https://www.youtube.com/watch?v=ByK8ADwI2mY

Site Oficial do Arduino IDE: https://www.arduino.cc/<br>
Projeto do Github do Arduino IDE 2.x: https://github.com/arduino/arduino-ide<br>
Site Oficial do Arduino Cloud: https://cloud.arduino.cc/<br>
Site Oficial do Arduino Web Editor: https://create.arduino.cc<br>
Site Oficial do Arduino IoT: https://create.arduino.cc/iot/things<br>
Site Oficial do Arduino Profile: https://id.arduino.cc/<br>
Site Oficial do Fritzing: https://fritzing.org/

#00_ Verificando as Informações do Sistema Operacional Linux Mint<br>

	Terminal: Ctrl + Alt + T

	#OBSERVAÇÃO IMPORTANTE: Linux Mint 20.x é derivado do Ubuntu Desktop 20.04.x Focal Fossa 
	#OBSERVAÇÃO IMPORTANTE: Linux Mint 21.x é derivado do Ubuntu Desktop 22.04.x Jammy Jellyfish
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

#02_ Plugar o Arduino na porta USB no Linux Mint<br>

	#OBERVAÇÃO: verificar se os LED's de indicação do Arduino começa a piscar

#03_ Clonar o Projeto do Github<br>

	git clone https://github.com/vaamonde/arduino

#04_ Acessando o diretório clocando do Arduino<br>

	cd arduino/

#05_ Executando o script de Instalação do Arduino IDE 2.x no Linux Mint<br>

	#INSTALAÇÃO DO ARDUINO IDE NO LINUX MINT 20.x
	bash install20.sh

	#INSTALAÇÃO DO ARDUINO IDE NO LINUX MINT 21.x
	bash install21.sh

#06_ Executando o Arduino IDE 2.x no Linux Mint<br>

	arduino-20

#07_ Verificando as Informações do Hardware do Arduino no Linux Mint<br>

	Arduino IDE 2.2.x
		Tools
			Board "Arduino Uno"
			Port: "/dev/ttyACM0"
			Get Board Info

#08_ Executando um projeto básico do Arduino IDE no Linux Mint<br>

	File
		Examples
			01. Basics
				Blink
					Upload

#09_ Verificando as Informações do Hardware do Arduino utilizando o Arduino-Cli<br>

	Terminal (Ctrl + Alt + T)
		arduino-cli
		arduino-cli version
		arduino-cli board list