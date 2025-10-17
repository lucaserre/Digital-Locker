# Digital-Locker
Se trata de um cofre digital, desenvolvido a partir de um desafio proposto pela instituição DIO.me, que envolvia a criação de um ransomware utilizando a linguagem python



Inicialmente, quis entender como um pentester executaria esse tipo de arquivo, visto que o existe a necessidade de ter o Python e suas respectivas bibliotecas instaladas. 
Então, pensei que seria um processo dificil de executar, já que exigiria o acesso à máquina da vítima, através de exploit, phisshing, etc. Escalonamento de privilégios. E, por fim a instalação de todas as ferramentas.
Porém, isso seria loucura. Seria como tentar arrombar a porta de uma casa com uma britadeira. Muito barulhento, seria demorado, deixaria rastros, aumentando a probabilidade de ser descoberto. 

Com isso, realizando pesquisas, descobri que poderia compilar um .exe, como se impacotassemos o ambiente todo em um único arquivo. Uma ferramenta que faz bem isso é o PyInstaller.

# PyInstaller:

Ele analisa o script Python (ransoware.py), identifica todas as bibliotecas que ele precisa (como a cryptography), e empacota tudo isso junto com um interpretador Python mínimo dentro de um único arquivo executável (.exe).
O resultado é um arquivo ransoware.exe que pode ser executado em qualquer computador Windows compatível, mesmo que ele não tenha o Python instalado. O arquivo é 100% autônomo!!!!!!!!!

A seguir é o processo de instalar a biblioteca e como compilar o script em um arquivo único:

    pip install pyinstaller

Depois:

    pyinstaller --onefile --noconsole ransoware.py

--onefile: Cria um único arquivo .exe em vez de uma pasta com vários arquivos. Essencial para portabilidade.

--noconsole (ou --windowed): Crucial para malwares. Isso garante que, quando o .exe for executado, nenhuma janela preta de terminal apareça na tela do usuário, fazendo com que ele rode de forma silenciosa e invisível em segundo plano.

--O PyInstaller cria uma pasta chamada dist. Dentro dela, você vai encontrar o seu ransoware.exe pronto para ser usado.



# Segurança

Nesse contexto, apesar de aprendermos a atacar, também precisamos aprender a nos defender, criando nossa própria política de segurança, mesmo que básica, evita muitos problemas.

----Não sair baixando conteúdo pirata, porque, além de anti-ético, também pode ser algum arquivo malicioso que prejudicará seu sistema. Então, evite ao máximo.
----Utilizar anti-vírus
----Alterar senha de acesso ao modem
----Alterar a senha do roteador para uma mais complexa e maior
----Criar uma senha de acesso para seu usuário
----Utilizar um usuário simples para questões do dia-a-dia e, caso exista a necessidade de um privégio maior, utilizar um usuário administrador
----Não compartilhar dados sensíveis, como senhas, números de telefone, ou até mesmo seus documentos
----Manter sempre o sistema Atualizado
----Utilizar um gerenciador de senhas para auxiliar na diversificação de senhas utilizadas para cada conta criada em suas respectivas plataformas. 
----Ativar o descanso de tela automático
----Cuidado com câmeras que pode ver a tela do seu computado, possibilitando a captura de dados sensíveis. 
----Realizar o escaneamento inteligente pelo menos uma vez na semana





# Ransomware


Parte 1:
<img width="1919" height="1035" alt="image" src="https://github.com/user-attachments/assets/8e9879a3-7103-4121-8941-0ee6d425dbe7" />

Parte 2:
<img width="1919" height="1031" alt="image" src="https://github.com/user-attachments/assets/74525f2a-7b3b-45c2-9eeb-e46eeae39573" />


# KeyLogger


Parte 1:
<img width="1919" height="1012" alt="image" src="https://github.com/user-attachments/assets/eeba7e7e-7b5e-421c-a158-dde1a34d60ed" />

Parte 2:
<img width="1919" height="1031" alt="image" src="https://github.com/user-attachments/assets/8376214c-f78a-4f9e-9d71-dc96f82929ff" />




# Pós crédito

Diante de tudo que aprendi no curso, o que mais me interessou e despertou uma ideia genuína, foi a última aula, em que aprendemos a desenvolver um ransomware, compreendendo como funciona, como se aplica e o mais importante, como se defender. 
Essa aula me fez pesquisar sobre uma área que gosto muito, principalmente por ter cursado Matemática Discreta na faculdade, que é a de criptografia. Então, pensei em como eu poderia utilzar ela pra se proteger. 
Então, ao invés de criptografar de maneira maliciosa, pensei que talvez seria uma boa ideia criptografar uma pasta inteira e possibilitar o acesso através de uma senha. Descobri que é possível, e se tornou minha maior dedidcação agora. 

Assim, inauguro hoje, o meu projeto particular: um cofre-digital, apelidado carinhosamente de Digital-Locker — pensei em Mind-Loker, mas talvez não fizesse tanto sentido — que se tornará uma forma de proteger os arquivos de uma pasta. 
Sei que o windows já faz isso, porém, em algumas versões isso não é habilitado, exigindo baixar softwares externos, como VeraCrypt — que fiquei fascinado de conhecer, pela sua complexidade e engenhosidade — que, apesar de ser muito bom, parece algo complexo demais para algo que exija uma ferramenta mais simples. 

Já iniciei esse processo. Então, espero o quanto antes desenvolver e receber auxilios. 

Obrigado! 



