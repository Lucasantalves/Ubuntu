WoeUSb é um fork do WinUSB. 
Ambos são open source e fazem pendive de boot no linux, mas o WinUSb não é atualizado desde 2012.
A inslação do WoeUSB precisa usar PPA para instalar nas versões 14.04/16.04/17.04.
Siga os comandos abaixo para adicionar a PPA.

# sudo add-apt-repository ppa:nilarimogard/webupd8

# sudo apt update

# sudo apt install woeusb

Caso queira remover o PPA siga os comandos:

# sudo add-apt-repository --remove ppa:nilarimogard/webupd8

# sudo apt update

Carregue o WoeUSB pelo dash ou pelo terminal com o comando:

# woeusbgui

Muito fáçil usar o WoeUSB.
Selecione a imagem do Windows e o dispositivo usb. 
Cuidado com os dados no pendrive antes de instalar.

Aguarde até terminar a instalação.
Concluído! Pode usar o pendrive de boot para instalar o Windows.

Como usar o WoeUSB pela linha de comando.

Primeiro procure o nome do pendrive como o comando a seguir:

# lsblk

No meu caso seria o sdb1

Desmonte o com o comando a seguir:

# sudo umount /dev/sdb1

Crie o pendrive de boot do Windows 10 com o comando a seguir:

# sudo woeusb -v --device windows-10.iso /dev/sdb

Pronto, agora você já sabe como criar facilmente um pendrive de boot do Windows 10 no Ubuntu ou qualquer outra distribuição Linux. Mas, um detalhe, não esqueça de ter um bom antivírus e um ótimo firewall ao usar o Windows, seja ela qual for a versão.
