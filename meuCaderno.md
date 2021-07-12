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