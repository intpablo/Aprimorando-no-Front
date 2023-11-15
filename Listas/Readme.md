#  LISTAS
O HTML fornece suporte para a representação visual de três tipos de listas: as ordenadas, as não ordenadas e as de definição.
1. Ordenadas
   - Usadas quando desejamos listar dados com a necessidade de representar a sua ordenação de forma numérica ou alfabética.
3. Não Ordenas
   - Usadas quando não há necessidade de listar ordenadamente.
5. De Definição
   - Usadas quando precisamos listar itens e atribuirmos uma descrição a eles.



 ⚠️ Outra característica importante das listas é que a sua marcação HTML é composta por uma tag de container, ou tag “pai”, e por seus itens ou “filhos”. Além disso, a lista de definição possui ainda um terceiro item, que é justamente o utilizado para descrevê-lo.

## 
| Tipo	  | Tag Container	 | Tag Item	    | Tag Descrição |
|-------------|-------------|-------------|-----------|
|Ordenadas    | `<ol>`      | ` <li> `     |-----------|
|Não Ordenadas|  `<ul> `       |`<li>`        |-----------|
| Definição   |`<dl>`        |  `<dt>`      |   `<dd>`    |

## Resultado das Listas    

### Lista Ordenada 
<ol>                                    
<li> Primeiro Item da lista </li>     
<li> Segundo Item da lista </li>    
<li> Terceiro Item da lista </li>
</ol>   
 
### Lista Não Ordenada 
<ul>
<li> Primeiro Item da lista não ordenada </li>
<li> Segundo Item da lista não ordenada </li>
<li> Terceiro Item da lista não ordenada </li>
</ul>

### Lista de definição 
<dl>
<dt> Primeiro Item da lista não ordenada </dt>
<dd> Descrição do primeiro elemento </dd>
<dt> Segundo Item da lista não ordenada </dt>
<dd> Descrição do segundo elemento </dd>
<dt> Terceiro Item da lista não ordenada </dt>
<dd> Descrição do terceiro elemento </dd>
</dl>
