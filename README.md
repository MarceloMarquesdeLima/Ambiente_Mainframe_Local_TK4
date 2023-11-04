# Ambiente Mainframe TK4

Sempre via necessidade de poder ter um ambiente para treinamento local com recursos de Mainframe e este será passo a passo rápido para configuração.

Baixar o repositório que contém todos os arquivos necessários para o ambiente:

“https://drive.google.com/drive/folders/14X1zuK38o36IQZgIdsb7soLUTkKKIDDj?usp=drive_link”

![image](https://github.com/MarceloMarquesdeLima/Ambiente_Mainframe_Local_TK4/assets/111276703/344352b1-352f-4926-b538-635fe7f4e99f)


Consultar o Guia TK4 — Passos para instalação e acesso que tem no repositório préviamente clonado;

Na raiz do windows criar uma C:\tk4 e dentro dela descompactar o arquivo tk4-_v1.00_current que contém no repositório;

Após descompactar vamos configure o TK4 no Windows no modo de execução para Console, como o prompt de comando vai até a pasta C:\tk4\unattended\ e execute set_console_mode.bat

Edite o arquivo de configuração que está na pasta c:\tk4\conf\tk4-.cnf e usando Bloco de Notas: Procure a chave: NUMCPU e mude de “1” para “2” - ${NUMCPU:=2} e da mesma forma procure a chave MAXCPU e mude de “1” para “2” - ${MAXCPU:=2} | já na opção CNSLPORT e veja a porta TCP/IP está ${CNSLPORT:=3270} | Na opção HTTPPORT e veja a porta TCP/IP está ${HTTPPORT:=8038}

Entre na pasta c:\tk4 pelo prompt de comando execute mvs.bat, aguarde até subir o serviço;

![image](https://github.com/MarceloMarquesdeLima/Ambiente_Mainframe_Local_TK4/assets/111276703/8cd53a82-607d-44de-9551-797d0ddfce11)

Terminou de subir o serviço ficar com está aparencia.
![image](https://github.com/MarceloMarquesdeLima/Ambiente_Mainframe_Local_TK4/assets/111276703/4d2c673a-1224-4ecf-b5d0-c6aca73bf407)

Instale o TN3270 ou Zoc e configure o acesso com o seu endereço IP local; criando uma conexão com a opção de emulador no TN3270 com IP de sua maquina local na porta 3270, Após confirmar que o serviço terminou a subida do item 6, conecte no terminal;
![image](https://github.com/MarceloMarquesdeLima/Ambiente_Mainframe_Local_TK4/assets/111276703/c9440163-6485-42c6-9567-ed9cf47b641d)

Conectando no serviço após configurar o terminal.
![image](https://github.com/MarceloMarquesdeLima/Ambiente_Mainframe_Local_TK4/assets/111276703/2257c08b-91db-488e-a667-330e974345be)

Após está conectado faça o Login conforme o Guia do TK4 e navegue pelo TSO/ISPF.
![image](https://github.com/MarceloMarquesdeLima/Ambiente_Mainframe_Local_TK4/assets/111276703/ced62593-1ee8-43a8-a04b-ab35c5fb1d17)

Encerre digitando logoff no terminal;

![image](https://github.com/MarceloMarquesdeLima/Ambiente_Mainframe_Local_TK4/assets/111276703/b364d2ca-7e2a-4b73-86e9-1bba2cca241c)

Para sair do Hercules emulador mainframe do MVS 3.8 digite: herc ===== exit

![image](https://github.com/MarceloMarquesdeLima/Ambiente_Mainframe_Local_TK4/assets/111276703/54b52b03-dbb4-402a-a861-93a4677923a1)

Encerrado de forma correta.

![image](https://github.com/MarceloMarquesdeLima/Ambiente_Mainframe_Local_TK4/assets/111276703/cb25f889-be34-409b-b62e-4653e02d6fcf)










