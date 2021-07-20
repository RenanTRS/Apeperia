# Aula01 - Ferramentas, unidades e imagens
## Introdução ao Emmet:
- Atalho para gerar tags html.  
```
header>img+nav>ul>li*3>a
```
```
<header>
	<img src="" alt="">
	<nav>
		<ul>
			<li><a href=""></a></li>
			<li><a href=""></a></li>
			<li><a href=""></a></li>
		</ul>
	</nav
</header>
```
## Aplicando estilos:
- Apenas a aplicação dos estilos.  

## Rem e Em:
- **rem** Varia de acordo com o valor da tag raiz ```<html>```.  
- **em** Varia de acordo a tag mãe.

# Aula02 - Layout mobile e Variáves CSS
## Viewport e seu conteúdo:
### Variáveis CSS:  
- São melhor usadas em seletores fortes, como ```:root{}```.  
```
:root {
	--branco: #fff;
	--montserrat: 'Montserrat', sans-serif;
}

color: var(--branco);
font-family: var(--montserrat);
```

# Aula03 - Particularidade de telas
## Unidades de medida Viewport:
- ```vw``` Unidade de medida em viewport que pode até transcender um padding e ocupar 100% da página.  
```
.container{
	width: 100vw;
}
```
## Medidas absolutas e relativas:
### O uso depende.
- ```max-width: 600px;``` Útil para elementos que precisam ser de tamanhos relativos em telas pequenas  mas para telas grandes não podem ser proporcionalmente do mesmo tamanho.  

# Aula04 - Trabalhando a semântica HTML
## Lidando com imagens:
- Se uma imagem não tem importância de conteúdo, não há necessidade dela estar no html, pode ser chamada via css.  
- Para colocar uma imagem via css:  
```background-image: url(../img/icone-relogio.png);```  
- Para não repetir:  
```background-repeat: no-repeat;```  
- Para posicionar:  
```background-position: top 1.25rem left 2.5rem;```  

## As tags address, video e br:
- Para colocar endereço:  
```<address></address>```  
- Para links abrirem apps de ligação:  
```<a href="tel:++551155712751">```  
- Para links abrirem apps de email:  
```<a href="mailto:contato@apeperia.com">```  

- Para colocar um vídeo:  
```<video src="diretorio" controls>``` **Controls** Serve para aparecer os controles de pause, barra de progresso e etc.  

# Aula05 - Evoluindo do mobile ao desktop
## Evoluindo o layout para tablet:  
- Para informar ao navegador o que fazer em determinado tamanho de tela:  
```
@media screen and (min-with:tamanho){
		Apenas o que será alterado;
}
```
- Mobile geralmente é: **375px**
- Tablet geralmente é: **768px**
- Desktop geralmente é: **1024px**

- Para imagem via css caber dentro do bloco:  
```background-size: cover;```  
- Para esconder um elemento via css:  
```display: none;```  