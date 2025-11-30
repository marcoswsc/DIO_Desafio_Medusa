# DIO_Desafio_Medusa
Este desafio teve o ituito de demonstrar o aprendizado sobre a ferramenta "MEDUSA", umas das ferramentas presentes no Kali Linux.
Repositório relacionado ao desafio do curso da DIO sobre Cybersecurity.

## Preparação do ambiente de laboratório:
  * Utilização do VirtualBox para virtualizar as máquinas;
  * Utilização do Kali Linux, como máquina atacante;
  * Utilização do Metasploitable2, como máquina alvo. O Metasploitable2 é uma máquina propositalmente vulnerável muito utilizada em estudos de técnicas em cibersegurança.  
OBS: Ao utilizar o Metasploitable2, utilize-a no virtualBox no mode de rede "Host-Only", para que a máquina não tenha contato com a rede do host.   

## Conhecendo a MEDUSA:
A MEDUSA é uma ferramenta de linha de comando presente na distribuição Kali Linux, muito utilizada em ataques de força bruta, desenvolvida para tentar descobrir credenciais com ponto de vulnerabilidade, ou seja, credenciais não fortes e não elaboradas.  
Essa ferramenta pode ser utilizada em diversos serviços, como FTP, SSH, HTTP (Principalmente formulários WEB), MySQL, RDP, POP, IMAP, Telnet, e outros.  
Sua utilização consiste em executar o comando, passando como parâmetros, o usário ou uma lista de possíveis usuários, o senha ou uma lista de possíveis senhas, o endereço do host ou endereço da máquina onde está o serviço o qual pretendemos testar e descobrir as credenciais.  
Ex: Tentativa de descobrir uma credencial no serviço FTP.  
comando: medusa -h {IP} -u {usuário} -P {senha} -M {ftp} -t {threads}  
-h: IP da máquian alvo;  
-u: usário ou lista de nomes de usuários;  
-P: senha ou uma lista de senhas;  
-M: serviço a ser testado, como FTP por exemplo.  
-t: Número de threads.  
OBS: Ao usar o comando acima, retire as chaves {}, apenas informa o necessário para utilização do comando.  
