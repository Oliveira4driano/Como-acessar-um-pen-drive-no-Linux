# Como-acessar-um-pen-drive-no-Linux

Como acessar um pen drive no Linux

No entanto, em Linux, um pen drive precisa ser montado como um sistema de arquivos. Coisas que você precisa superusuário (root) password Show Mais instruções 

1 - o botão direito do clique com o mouse na área de trabalho e selecione "Terminal Open" no menu pop- up menu. 

2- Digite " su " e pressione " Enter". Em seguida, digite sua senha de root e pressione "Enter " para obter administrador ( root) privilégios. 

3- Digite " cd /mnt " e pressione " Enter". 
 
4 - Digite "mkdir usb " e pressione " Enter" para criar um diretório USB. 

5- Digite " cd /etc " e pressione " Enter". 
 
6- Digite " cp fstab fstab_original " e pressione " Enter" para fazer backup do arquivo fstab originais. 

7- Tipo " nano fstab " e pressione " Enter" para editar o arquivo fstab. 

8- Adicione a seguinte linha no final do arquivo fstab no editor nano:
/dev/sdc1 /mnt/usb auto noauto,user,rw 0 0 

9- Para gravar as alterações pressione: CTRL+O depois CTROL+X para sair do editor nano. 

10- Digite "exit " e pressione "Enter " para sair do shell.Note root: . Passos 2 a 10 são apenas uma one- processo de tempo . Uma vez que eles são feitos, sempre começar a partir do Passo 11 . 

11- Insira um pen drive em uma porta USB. 

12- Digite " mount  /mnt/usb" e pressione " Enter". 

13- Digite " cd  /mnt/usb" e pressione " Enter". Digite " ls " e pressione " Enter" para listar o conteúdo de pen drive . 

14- Clique no ícone da pasta USB , que deve aparecer na área de trabalho , para acessar o conteúdo da unidade. 

15- Desmonte um pen drive , fechando todos os arquivos e pastas que foram utilizados na unidade. 

16- Tipo " umount  /mnt/usb" e pressione " Enter". 

17- Remover o pen drive da porta USB . 
