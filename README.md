# MP_producoes



Este site é referente a uma empresa que pra já é fictícia, do ramo de designer de interiores e de obras. A tal empresa ainda está nos planos de um familiar, mas aproveitei da ideia para já testar websites, propagandas e afins. Para este projeto, a minha principal referência foi o website da empresa Rima (https://www.rimadesign.pt), outra empresa de design de interiores. O site tem uma proposta mais minimalista, elegante e clean, o que evidencia o público alvo e o estilo da propria empresa. Tentei trazer um pouco desta abordagem tambem ao codigo e ao website deste projeto. 

INDEX: Na página inicial, ou seja, no index.html, o utilizador concontra uma barra de menu, o header, que possui opções mais genericas no canto esquerdo (quem somos, nossos serviços e galeria). NO centro desse menu está posicionada a logo da empresa e no canto direito, destacado, está a opção de "Contactos". Optei por separar esta opção porque acredito que os utilizadores tem maior tendencia em levar os olhos pro canto direito, num item que está isolado, por isso, poderia haver maiores possibilidades de clicar na opção de contactos, para assim, movimentar as redes da suposta empresa. Nesta barra de menu, todas essas opções correspondem a buttons, quem levam o utilizador a outra página. Para isso, foi usada a <a href = "nome da pagina">, salvo a imagem da logo que teve dentro do href uma imagem src, já que a logo corresponde a um arquivo png. Abaixo da barra de menu, há outra <div> chamada intro-section, com o slogan da empresa e uma frase apresentativa, para já dar a entender sobre o que se trata aquele website. Para além disso, no corpo do site, vê-se um video no canto direito que está com os comandos de <autoplay e loop>, para que o video inicie automaticamente toda vez que o utilizador acessar o index.html, e o loop para que o video esteja sempre a dar enquanto o utilizador lá permanecer. Ao lado do video, há um conteiner com uma mancha de texto. Esses itens estão dentro de uma div principal que se chama container, mas cada item está tambem dentro de outra div, de forma separada, para que fosse possivel da-los estilos diferentes das demais funções do website. Após esse container do video-section, próximo ao rodapé, é possivel ver uma animação feita com javascrip, que envolve imagens e textos. Essa animação consiste em trocar imagens e textos simultaneamente a cada 4 segundos, com um leve fade in e fade out entre as trocas. A nivel de html, as imagens e textos estão dentro de uma div que se chama slideshow-container e dentro desta div, foram atribuidos ids para as imagens,pros titulos e para os textos, pois assim, o script consegue identificar os item atraves do getElementarybyId, possibilitando a lógica do código e tornando a animação possível. Como são 3 imagens, a lógica identifica a primeira imagem com o index 0 e a cada 4 segundos (tempo determinado tambem no codigo), ele assume indox0+1, mudando para a proxima imagem. Depois temos neste script o @keyframe do fadeEffect, para que a imagem nao seja trocada de forma tão brusca, tornando o efeito mais agradável e sutil.  Depois desta animação, decidi pôr um botão que leva o utilizador a um pequeno quizz de estilos de design, para que o site tenha uma experiencia mais interativa. O quizz é simples, de apenas 5 perguntas, apenas para criar algo diferenciado. A unica forma de acessar o quizz seria pela pagina index.html e clicar no botao ao fim da pagina, pois não há a opção do quizz na barra de menu. 
Depois do botao do quizz, há o rodapé, footer, que possui uma posição fixa e que assim como a barra de menu, estará presente em todas as páginas deste website. Esse rodapé está em uma div, que possui nela texto e links que levam o utilizador as principais redes sociais que são utilizadas hoje em dia. Não pus nenhuma rede social em especifico porque a empresa como não existe, também não possui redes sociais, mas para que os links funcionem, inseri a pagina de login em cada uma das redes, logo, quando o utilizador clica no link, ele será redirecionado à pagina de login da rede social clicada.
OBS.: foram inseridos Media Queries no código para que o mesmo seja responsivo aos diferentes formatos de ecrã. A responsividade não ficou incrivel, mas quando tentei mudar, prejudicou o site em desktop. POrtanto optei por deixar da forma como está porque de todas as tentativas, essa foi a que menos modificou as caracteristicas do website para desktop.  

QUIZZ: Na página do quizz, é possivel identificar na mesma a barra de menu e o rodapé, que são recorrentes em todas as páginas. No corpo/main desta pagina, tenho a div do quizz-container que aplica Id as diferentes funções necessárias para que a animação seja feita. Nesta pagina o java reconhece os Ids atraves do getElementarybyId. As Ids incluem perguntas, respostas e pontuação. A cada resposta o utilizdor soma uma pontuação diferente, o que permite ao codigo fazer a soma dessas pontiações para que ao fim da quinta pergunta o código consiga encontrar a solução do quizz. São 3 resultados possiveis ao fim e a logica diz que de 0-6= resultado x, de 6-10= resultado y, else= resultado z. Após a aparição do resultado, há uma alimação de firework que aparece, isso se dá porque foi atribuido uma class e uma id= firework. Por isso o script chama esta Id e faz a animação ocorrer por 3 segundos. A animação traz a lógica matematica randon tando no tamanho, quando nas cores, trazendo o dinamismo dos fireworks. Após a aparição do resultado, surge o botao de refazer teste restartQuizz (), que quando clicado, o teste volta pro inicio. O utilizador pode fazer o teste quantas vezes quiser. E ele só sairá daquela página se utilizar a barra de menu na parte superior do website. 

QUEM SOMOS: Esta página é razoavelmente simples a nivel de códigos. Ela consite em dois blocos com duas divs que contem uma imagem e uma mancha de texto. Na div principal de cada bloco, possui uma imagem, e depois há outra div onde possui a manda de texto. O texto fala um pouco da historia de cada um dos envolvidos na empresa, cuja fotografia os identifica. A única novidade desta página é a presença do .divider, que atribui duas linhas para separar um bloco do outro. As linhas receberam suas caracteristicas, tais como, cor e tamanho, no css <style>. Por fim, antes do rodapá, há um botão "Ver mais", que leva o utilizador à pagina galeria.html. No mais, a página possui os mesmos codigos das outras, como a barra de menu e o rodapé. 

GALERIA: Esta página é onde era suposto mostrar os trabalhos da empresa. Por não ser uma empresa real, as fotos foram retiradas da plataforma pexels para ilustrar como seria. E também não tenho aqui muitas fotos. Utlizei um todas de 5 fotografias, apenas para ilustrar como seria esta sessão do site num cenário real. Nesta página, para além da barra de menu e do rodapé, que estão sempre presentes, há um container onde a foto é exposta e uma animação que consiste na presenta de setas para que o utilizador possa navegar pela galeria. A animação é feita através do script onde foi atribuida uma classe para seta esquerda/seta direita e onde  a primeira foto foi atribuida. Sendo assim, a logica permite que toda vez que a seta direita tenha um clique o indice muda da foto 1 para 1+1, trocando assim a foto. A logica faz, também, o sentido contrário quando a seta esquerda é clicada. Sendo assim, o site fica mais interativo e o utilizador consegue mudar a foto para frente e para trás. Essa amimação não há fim, por isso, o utilizador só sairá desta página se recorrer a barra de menu na parte superior do site. No fim, há um botão "Fale Connosco" que quando clicado, levará o utilizador à página contactos.html


NOSSOS SERVIÇOS: Esta página assemalha-se um pouco com a página quemsomos.html a nivel de codigo, pois não há javascript. Aqui há apenas html e css. Esta página consiste em dois blocos principais onde em cada um desses blocos há 6 imagens verticais lado a lado e por debaixo dessas imagens, em outra div, há uma mancha de texto para falar um pouco mais sobre os serviços prestados pela empresa. As fotografias possuem um width de 15% e uma height auto para que fiquem menores e para alem disso possuem border radious para que fiquem ligeiramente arredondadas nas pontas e possuem tambem um drop shadow para pareça "saltar", de forma sutil, da página. Os dois blocos possuem o mesmo codigo, o que muda são as imagens expostas de um bloco para o outro, assim como o conteudo do texto.  No fim,há um botao que diz "Agende uma visita". Após clicar nesse botao o utilizador é levado a pagina de contactos.html. No mais, a barra de menu, com o container do titulo da pagina e o rodapé, permanecem lá como em todas as outras paginas. 


CONTACTOS: Nesta página, há a presença do php para tornar a pagina interativa ao ponto do utilizador poder escrever o nome,apelido e tambem enviar uma mensagem que apareça automaticamente no email da empresa. Eu fiz o teste do codigo, mas acho que não funciona tão bem. No entanto, não consegui melhorar de forma que o tornasse possivel. Ao cnto esquerdo, tem os links das redes sociais e o numero de contacto. No mais, há na mesma a barra de menu e o rodapé com as mesmas caracteristicas. 

Para concluir, penso que a primicia da ideia está presente. E que o site em geral está visualmente agradável e que o mesmo possui uma certa interação com o utilizador. Acredito que muito poderia ser feito para melhorar, principalmente o tipo da fonte e o tamanho, pois me parece que por vezes as fontes não parecem pertencer aquele site. Tive certa dificuldade em encontrar ou identificar um tipo de letra que me parecesse bem. Penso que tambem mudaria o layout de uma pagina ou outra, como por exemplo a pagina "nossos serviços", que parece simples e feita por uma pessoa inexperiente, o que de fato é, mas nao era a intençao parecer que sim. Outra coisa que deveria melhorar seria a responsividade do site, porque embora esteja no codigo, sinto que não ficou tão bem como eu gostaria. No mais, penso que as principais ideias estão presentes. 
