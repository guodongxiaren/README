README
===========================

Este arquivo é usado para testar e exibir várias sintaxes de remarcação para escrever o README。A sintaxe de markdown do GitHub está no padrão markdown Estendido gramaticalmente，chame-o`GitHub Flavored Markdown`。Abreviação`GFM`，O GFM é amplamente usado no GitHub，Exceto para arquivos README, ambos os problemas e a sintaxe de marcação de suporte do wiki.

****


|Autor|Camarão Jelly|
|---|---
|Saber|[![zhihu-escudo]][zhihu]
|Conta pública|Histórico de programação


****
## Índice
* [linha horizontal](#linha horizontal)
* [título](#título)
* [texto](#texto)
    *texto normal
    * texto de linha única
    * Texto multilinha
    * destaque de texto
    * nova linha
    * itálico
    * negrito
    * tachado
* [Imagem] [imagem)
    *Fotos da Internet
    * Imagem do repositório GitHub
* [link](#link)
    * hiperlink de texto
        * link URL externo
        * Link para a URL neste repositório
    * ponto de ancoragem
    * [link da imagem](#link da imagem)
* [lista](#lista)
    * lista não ordenada
    * lista ordenada
    * lista de caixas de seleção
* [blockquote](#blockquote)
* [destaque de código](#destaque de código)
* [tabela](#tabela)
* [expressão](#expressão)
* [sintaxe do diferencial](#sintaxe do diferencial)
* [Sintaxe HTML comum](#Sintaxe HTML comum)
    * [dobrar](#dobrar)
    * [centralizado](#centralizado)
* [outro](#outro)
    * [crachá](#crachá)
    * [histórico das estrelas] (#histórico das estrelas)

### Linha horizontal
-----------
***, ---, ___ pode exibir efeito de linha horizontal

***
---
___



## título
```
# Título de nível 1
## Título de segundo nível
### Título de nível 3
#### Títulos de nível 4
##### Título de Nível 5
###### Nível 6 Cabeçalho
```
O efeito é o seguinte:

# Título de nível 1
## Título de segundo nível
### Título de nível 3
#### Títulos de nível 4
##### Título de Nível 5
###### Nível 6 Cabeçalho


## texto
### texto simples
Este é um texto normal
### Texto de linha única
    Olá a todos, sou Jelly Shrimp.
Adicione 1 tabulação ou 4 espaços no início de uma linha.
### blocos de texto
#### Sintaxe 1
Adicione 1 tabulação ou 4 espaços no início de várias linhas consecutivas de texto.
bem-vindo a visitar
    prazer em conhecê-la
    Desejo-lhe bom dia, bom meio-dia, boa tarde e boa noite

#### Sintaxe 2
Use um par de três acentos graves:
```
bem-vindo a visitar
Eu sou um codificador C++
Você pode pesquisar [Jelly Shrimp] em Zhihu, CSDN e Jianshu para me encontrar
```
Essa sintaxe também pode obter realce de código, consulte [destaque de código](#destaque de código)
### destaque de texto
A função de destaque de texto pode destacar parte do texto na linha, usando um par de acentos graves.
gramática:
```
`linux` `programação de rede` `socket` `epoll`
```
Efeito: `linux` `programação de rede` `socket` `epoll`

Também adequado como tag para um artigo
#### Nova linha
O retorno de carro direto não pode mudar de linha,
Você pode adicionar dois espaços após a linha de texto anterior,
Isso irá quebrar o texto na próxima linha.

Ou apenas adicione uma linha em branco diretamente entre as duas linhas de texto.

O efeito de quebra de linha também pode ser obtido, mas o espaçamento entre linhas é um pouco grande.
#### itálico, negrito, tachado

|Sintaxe|Efeito|
|----|-----|
|`*Itálico 1*`|*Itálico 1*|
|`_Itálico 2_`| _Itálico 2_|
|`**Negrito 1**`|**Negrito 1**|
|`__bold 2__`|__bold 2__|
|`Este é um ~~riscado~~`|Este é um ~~riscado~~|
|`***Itálico Negrito 1***`|***Itálico Negrito 1***|
|`___Itálico Negrito 2___`|___Itálico Negrito 2___|
|`***~~Itálico Negrito Riscado 1~~***`|***~~Itálico Negrito Riscado 1~~***|
|`~~***Itálico negrito tachado 2***~~`|~~***Itálico negrito tachado 2***~~|

    Itálico, negrito, tachado podem ser misturados

## foto
Formato básico:
```
![alt](título do URL)
```
alt e title correspondem aos atributos alt e title em HTML (ambos podem ser omitidos):
- alt indica o texto de substituição quando a exibição da imagem falha
- título indica o texto de exibição quando o mouse passa sobre a imagem (observe que as aspas são necessárias aqui)

URL é o endereço url da imagem. Se você se referir à imagem neste depósito, pode usar diretamente **caminho relativo**. Se você se referir à imagem em outros depósitos do github, preste atenção ao formato, que é: `endereço do armazém/bruto/nome da filial/caminho da imagem`, como:
```
https://github.com/guodongxiaren/ImageCache/raw/master/Logo/foryou.gif
```

|#|Sintaxe|Efeito|
|---|---|----
|1|`![baidu](http://www.baidu.com/img/bdlogo.gif "Logotipo do Baidu")`|![baidu](http://www.baidu.com/img/bdlogo. gif "logotipo Baidu")
|2|`![][código-past]`|![][código-past]

Observe que o método de escrita do Exemplo 2 usa a forma de **identificador de URL**, que é apresentado na seção [Link](#Link).
> Há uma definição de code-past no final do artigo:
```
[code-past]:/img/codepast-logo.jpg "Conta Oficial: Programação Passada"
```

## Link
### URL externo do link

|#|Sintaxe|Efeito|
|---|----|-----|
|1|`[Meu blog](http://blog.csdn.net/guodongxiaren "Hover Display")`|[Meu blog](http://blog.csdn.net/guodongxiaren "Hover Display")|
|2|`[Meu Zhihu][zhihu] `|[Meu Zhihu][zhihu]|

A sintaxe 2 consiste em duas partes:
- A primeira parte usa dois colchetes. O identificador em [ ] (zhihu neste exemplo) pode ser uma combinação de números, letras, etc., e os identificadores superior e inferior precisam corresponder (**vamos chamá-lo de identificador de URL* *)
- A segunda parte marca o URL real.

>O uso de identificadores de URL pode atingir o objetivo de reutilização.Geralmente, todos os identificadores de URL no texto completo são colocados no final do artigo, o que parece mais limpo. Além de ser limpo, também pode atingir o objetivo de reutilização. Por exemplo, se você deseja usar o mesmo link em vários lugares, use o identificador no texto e defina apenas o link de URL real para o identificador no inferior, semelhante a Variáveis ​​em linguagens de programação.
>> O identificador de URL é meu nome, não sei se é preciso. Ops. .

### Link para a URL neste repositório

|Sintaxe|Efeito|
|----|-----|
|`[Meu perfil](/exemplo/profile.md)`|[Meu perfil](/exemplo/profile.md)|
|`[exemplo](./exemplo)`|[exemplo](./exemplo)|

### link da imagem
A essência de vincular imagens é misturar a sintaxe de exibição de imagem com a sintaxe de link normal. Em um link normal, dentro de [ ] está o texto a ser exibido no link, enquanto em um link de imagem [ ] está a imagem a ser exibida.
É claro que é possível misturar diretamente as duas sintaxes, mas é muito detalhado, então podemos usar a forma de identificadores de URL.

|#|Sintaxe|Efeito|
|---|----|:---:|
|1|`[![weibo-logo]](http://weibo.com/linpiaochen)`|[![weibo-logo]](http://weibo.com/linpiaochen)|
|2|`[![](/img/zhihu.png "Meu Zhihu, bem-vindo a seguir")][zhihu]`|[![](/img/zhihu.png "Meu Zhihu, bem-vindo a seguir ") ][zhihu]|
|3|`[![csdn-logo]][csdn]`|[![csdn-logo]][csdn]|

Como a própria imagem e o próprio link suportam a forma de identificadores de URL, os links de imagem também podem ser concisos (consulte o Exemplo 3).
Observe que o texto exibido quando o mouse passa é o título da imagem, não o título do link em si.
> Os identificadores de URL deste artigo são colocados no final do artigo

### Âncora
Na verdade, cada título é um ponto de ancoragem, que é semelhante ao ponto de ancoragem (`#`) em HTML. Por exemplo, nós

|Sintaxe|Efeito|
|---|---|
|`[voltar ao início](#readme)`|[voltar ao início](#readme)|

Observe, no entanto, que as letras em inglês no título foram convertidas em **letras minúsculas**.
> No passado, o GitHub não suportava bem o chinês, então o título chinês não podia ser reconhecido corretamente como um ponto de ancoragem, mas agora não há problema!

## Lista
### Lista não ordenada
#### gramática
```
* Apelido: Jelly Shrimp
- Alias: Faraó ao lado
* Nome em inglês: Jelly
```
#### Efeito
* Apelido: Jelly Shrimp
- Alias: Faraó ao lado
* Nome em inglês: Jelly

### Lista não ordenada de vários níveis
#### gramática
```
* Linguagem de programação
    * linguagem de script
        *Pitão
```
#### Efeito
* Linguagem de programação
    * linguagem de script
        *Pitão

### Lista ordenada nível 1
#### gramática
Basta adicionar um ponto e um espaço após o número. Pode não ser óbvio o suficiente, no entanto.
```
Três características básicas da orientação a objetos:

1. Embalagem
2. Herança
3. Polimorfismo
```

#### Efeito
Três características básicas da orientação a objetos:

1. Embalagem
2. Herança
3. Polimorfismo


### Lista ordenada de vários níveis
Assim como as listas não ordenadas, as listas ordenadas também possuem uma estrutura de vários níveis.
#### gramática
```
1. Esta é uma lista ordenada de primeiro nível, o número 1 ainda é 1
   1. Esta é uma lista ordenada de segundo nível e os algarismos arábicos são exibidos como algarismos romanos
      1. Esta é uma lista ordenada de três níveis e os números são alterados para letras em inglês quando exibidos
```

#### Efeito

1. Esta é uma lista ordenada de primeiro nível, o número 1 ainda é 1
   1. Esta é uma lista ordenada de segundo nível e os algarismos arábicos são exibidos como algarismos romanos
      1. Esta é uma lista ordenada de três níveis e os números são alterados para letras em inglês quando exibidos


### lista de caixas de seleção
#### gramática
```
- [x] Análise de Requisitos
- [x] Projeto do Sistema
- [x] Projeto detalhado
- [ ] codificação
- [ ] teste
- [ ] Entrega
```
#### Efeito

- [x] Análise de Requisitos
- [x] Projeto do Sistema
- [x] Projeto detalhado
- [ ] codificação
- [ ] teste
- [ ] Entrega

Você pode usar esse recurso para marcar a conclusão das tarefas de um projeto.
> Dica:
>> Usar esta sintaxe no **problema** do GitHub pode clicar na caixa de seleção para marcá-la ou desmarcá-la em tempo real sem modificar o texto original do problema.

## bloco de citação

### Frequentemente usado para citar texto
#### O texto foi extraído de "In-depth Understanding of Computer Systems" P27
É incrível como as pessoas são emotivas sobre qual endianidade é apropriada. Os termos "little endian" e "big endian" vêm do livro de Jonathan Swift, Gulliver's Travels, onde duas facções em guerra não conseguem decidir de qual lado quebrar um ovo cozido. O debate, portanto, degenera em uma discussão sobre sociopolítica. Desde que uma regra seja escolhida e respeitada de forma consistente, a escolha da ordem de bytes é na verdade arbitrária.
> **Origem de "endian"**
Aqui está a descrição de Jonathan Swift da história da disputa endianness em 1726:
"... A próxima coisa que quero dizer é que as duas grandes potências Lilliput e Blefuscu têm lutado amargamente nos últimos 36 meses. A guerra começou pelo seguinte motivo: todos nós acreditamos que antes de comer ovos, a maneira primitiva é quebrar a ponta maior do ovo, mas o avô do atual imperador comeu ovos quando era criança e quebrou um dedo ao quebrar os ovos de acordo com o método antigo, então seu pai, o imperador da época , emitiu um decreto ordenando que todos os indivíduos comessem ovos. Quebre a ponta menor do ovo e os infratores serão multados pesadamente.

### Blockquotes têm vários níveis
#### gramática
```
> Estrutura de Dados
>> árvore
>>> Árvore binária
>>>> árvore binária balanceada
>>>>> árvore binária completa
```
#### Efeito
> Estrutura de Dados
>> árvore
>>> Árvore binária
>>>> árvore binária balanceada
>>>>> árvore binária completa

## realce de código

### gramática
Adicione o nome da linguagem de programação após os três acentos graves, comece a escrever o código em uma nova linha e adicione três acentos graves à última linha.

### Efeito
```Java
public static void main(String[]args){} //Java
```
```c
int main(int argc, char *argv[]) //C
```
```Bash
echo "olá GitHub" #Bash
```
```javascript
document.getElementById("myH1").innerHTML="Bem-vindo à minha página inicial"; //javascipt
```
```cpp
string &operator+(const string& A, const string& B) //cpp
```
## Folha
Cabeçalho 1 | Cabeçalho 2 |
--------- | --------|
Células de tabela |Células de tabela |
Células de tabela |Células de tabela |

| Cabeçalho 1 | Cabeçalho 2 |
| ---------- | -----------|
| Células da Tabela | Células da Tabela |
| Células da Tabela | Células da Tabela |

### alinhamento
As tabelas podem especificar o alinhamento

| Alinhar à Esquerda | Centralizar | Alinhar à Direita |
| :------------ |:---------------:| -----:|
| col 3 é | algum texto prolixo | $ 1600 |
| col 2 é | centrado | $12 |
| listras de zebra | são legais | $ 1 |

### misturar outra sintaxe
O conteúdo nas células da tabela pode ser usado com a maioria das outras sintaxes do GFM, como:
#### Use tachado, itálico e outros efeitos de texto comum

| Nome | Descrição |
| ------------- | ----------- |
|Ajuda |~~Mostra a~~ janela de ajuda.|
| Fechar | _Fecha_ uma janela |

#### Incorporar imagens (links) em tabelas
Na verdade, quando introduzimos a exibição de imagem e os links de imagem anteriormente, eles foram exibidos na tabela para maior clareza.

|imagem |descrição |
| ---- | ---- |
|![baidu][baidu-logo] |Baidu|

## expressão
A sintaxe Markdown do Github suporta a adição de expressões emoji. Inserir diferentes códigos de símbolo (caracteres cercados por dois-pontos) pode exibir diferentes expressões.

Por exemplo, `:blush:` pode exibir :blush:.

Para o código do símbolo de cada emoticon, você pode verificar a página oficial do GitHub [http://www.emoji-cheat-sheet.com](http://www.emoji-cheat-sheet.com).

Mas esta página abre **extraordinariamente lenta** todas as vezes. . Então, organizei-o neste repositório e você pode visualizar diretamente [emoji](./emoji.md) aqui.

## sintaxe diferente
A função diff é indispensável no sistema de controle de versão, ou seja, para exibir a adição e exclusão de conteúdo de um arquivo.
O efeito de diferença de exibição que pode ser exibido no GFM. Use verde para adições e vermelho para exclusões.
#### gramática
Sua sintaxe é semelhante ao realce de código, basta escrever diff após três acentos graves,
E em seu conteúdo, você pode usar o início de `+` para indicar adição e o início de `-` para indicar exclusão.
Há também sintaxe com `!` e `#`.

#### Efeito

``` diferença
+ O osmanthus de cheiro doce cai quando as pessoas estão ociosas,
- A noite é tranquila, as montanhas ficam vazias na primavera.
!
# Quando Ming Chunjian.
```
## Sintaxe HTML comum
Markdown suporta sintaxe HTML. Embora um grande número de sintaxe HTML não seja encorajado, afinal, ele perderá o significado de markdown, mas há algumas sintaxes HTML que raramente são adicionadas ao escrever o README.
### dobrar
```
<details>
<summary>Linux环境</summary>


##### compilar
xxxx

##### Instalar
xxxx
```
<details>
<summary>Linux arredores</summary>

##### compilar
xxxx

##### Instalar
xxxx
</details>

### Centralização

O efeito de centralização é usado em muitos lugares. Por exemplo, o conteúdo a seguir exibirá uma tabela no centro da página:

```
<div align="center">

| Cabeçalho 1 | Cabeçalho 2 |
| ---------- | -----------|
| Células da Tabela | Células da Tabela |
| Células da Tabela | Células da Tabela |

</div>
```

<div align="center">

| Cabeçalho 1 | Cabeçalho 2 |
| ---------- | -----------|
| Células da Tabela | Células da Tabela |
| Células da Tabela | Células da Tabela |

</div>

Qualquer outra sintaxe que precise ser exibida no centro pode ser colocada nela.

## outro
Há também algumas sintaxes não remarcadas, mas também componentes úteis em arquivos README.
### distintivo
Para desenhar insígnias, a primeira escolha é [shields.io](https://shields.io/)  Para gramática específica, acesse o site oficial para explorar.

![LICENSE](https://img.shields.io/badge/license-MIT-green)
![Author](https://img.shields.io/badge/Author-guodongxiaren-blue.svg)
![zhihu-shield]

Em segundo lugar, algumas plataformas de terceiros também fornecem emblemas convenientes, como gitter:

[![Join the chat at https://gitter.im/guodongxiaren/README](https://badges.gitter.im/guodongxiaren/README.svg)](https://gitter.im/guodongxiaren/README?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

### história da estrela
histórico de estrelas pode usar este site [star-history.com](https://star-history.com/)
```
[![Star History Chart](https://api.star-history.com/svg?repos=guodongxiaren/README&type=Date)](https://star-history.com/#guodongxiaren/README&Date)
```
O efeito de exibição desse código é o seguinte:

[![Star History Chart](https://api.star-history.com/svg?repos=guodongxiaren/README&type=Date)](https://star-history.com/#guodongxiaren/README&Date)


--------------------------------
[csdn]:http://blog.csdn.net/guodongxiaren "meu blog"
[zhihu]:https://www.zhihu.com/people/guodongxiaren "Meu Zhihu, bem-vindo para prestar atenção"
[weibo]:http://weibo.com/linpiaochen
[baidu-logo]:http://www.baidu.com/img/bdlogo.gif "logotipo Baidu"
[weibo-logo]:/img/weibo.png "Clique na imagem para entrar no meu Weibo"
[csdn-logo]:/img/csdn.png "Meu blog CSDN"
[code-past]:/img/codepast-logo.jpg "Conta Oficial: História da Programação"
[zhihu-shield]:https://img.shields.io/badge/dynamic/json?color=0084ff&logo=zhihu&label=%E6%9E%9C%E5%86%BB%E8%99%BE%E4%BB%81&query=%24.data.totalSubs&url=https%3A%2F%2Fapi.spencerwoo.com%2Fsubstats%2F%3Fsource%3Dzhihu%26queryKey%3Dguodongxiaren
