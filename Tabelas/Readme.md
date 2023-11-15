# Estrutura das Tabelas
- A marcação HTML relacionada às tabelas contém, além da tag principal <table>, outras tags. A principal define o container geral.
- De forma hierárquica, a seguir temos as tags para a definição de linhas `<tr>` e colunas `<td>`. Com estas três tags é possível representarmos uma tabela simples. Entretanto, há tags adicionais que podem ser usadas e que ajudam a melhor organizar o conteúdo.
- A tabela abaixo apresenta as tags de marcação, e suas respectivas funções, relacionadas às tabelas:

| Tag        | Função                                                                                                  |
|------------|---------------------------------------------------------------------------------------------------------|
| `<table>`  | Container principal da tabela                                                                          |
| `<tr>`     | Representa as linhas, sendo composta pelas tags relacionadas às colunas.                                |
| `<td>`     | Representa as colunas e precisa ser inserida dentro da tag de linha.                                   |
| `<th>`     | Representa colunas e é usada para exibir o título de uma coluna. Possui função semântica e estilos próprios. Deve estar contida em uma tag de linha. |
| `<thead>`  | Armazena o cabeçalho da tabela, composto por linhas e colunas. Tem função semântica na estruturação de conteúdo. |
| `<tfoot>`  | Armazena o rodapé da tabela, tendo função semântica na estruturação.                                    |


- As tabelas, normalmente, são organizadas de maneira uniforme: linhas sobre linhas, colunas após colunas, célula ao lado de célula. Logo, as colunas costumam ter a mesma largura, assim como as linhas a mesma altura. Entretanto, há situações onde é preciso mudar um pouco essa organização. Por exemplo, pode ser necessário mesclar duas colunas ou mesmo duas ou mais linhas.
Para isso, fazemos uso de alguns atributos - que têm função de destaque ao tratarmos das tags relacionadas às tabelas. São eles: **rowspan** e **colspan**. Como o próprio nome indica, estes atributos têm a função de expandir as linhas ou colunas. Sua declaração é acompanhada de um número que indica a quantidade de células a serem utilizadas para expansão da linha ou coluna.

# Tabelas em HTML

Este é um exemplo de código HTML que demonstra diferentes tipos de tabelas.

## Tabela Simples
<body>
    <table width="100%" border="1">
        <tr>
            <td>Alex</td>
            <td>HTML</td>
            <td>10</td>
        </tr>
        <tr>
            <td>Ana</td>
            <td>HTML</td>
            <td>10</td>
        </tr>
    </table>
</body>


<details> 
<summary> Mostrar Código HTML </summary>

 ``` html
    <table width="100%" border="1">
        <tr>
            <td>Alex</td>
            <td>HTML</td>
            <td>10</td>
        </tr>
        <tr>
            <td>Ana</td>
            <td>HTML</td>
            <td>10</td>
        </tr>
    </table>
```
</details>

## Tabela com Título 
 <table width = "100%" border = "1">
        <tr>
            <th>Aluno</th>
            <th>Disciplina</th>
            <th>Nota</th>
        </tr>
        <tr>
            <td>Alex</td>
            <td>Html</td>
            <td>10</td>
        </tr>
        <tr>
            <td>Ana</td>
            <td>Html</td>
            <td>10</td>
        </tr>
    </table>
<details>
  <summary>Mostrar Código HTML</summary>
  
  ```html 
   <table width = "100%" border = "1">
        <tr>
            <th>Aluno</th>
            <th>Disciplina</th>
            <th>Nota</th>
        </tr>
        <tr>
            <td>Alex</td>
            <td>Html</td>
            <td>10</td>
        </tr>
        <tr>
            <td>Ana</td>
            <td>Html</td>
            <td>10</td>
        </tr>
    </table>
  ```
</details>

## Tabela com Cabeçalho e Rodapé 
<table width = "100%" border = "1">
            <thead>
                <tr>
                    <th>Mês</th>
                    <th>Horas/Aula</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Junho</td>
                    <td>40</td>
                </tr>
                <tr>
                    <td>Julho</td>
                    <td>30</td>
                </tr>
            </tbody>
            <tfoot>
                <tr>
                    <td>Total</td>
                    <td>70</td>
                </tr>
            </tfoot>
          </table>

  <details>
    <summary>Mostrar Código HTML</summary>

    
  ```html 
   <table width = "100%" border = "1">
            <thead>
                <tr>
                    <th>Mês</th>
                    <th>Horas/Aula</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Junho</td>
                    <td>40</td>
                </tr>
                <tr>
                    <td>Julho</td>
                    <td>30</td>
                </tr>
            </tbody>
            <tfoot>
                <tr>
                    <td>Total</td>
                    <td>70</td>
                </tr>
            </tfoot>
          </table>
  ```
  </details>

## Tabela com Colspan 
<table widht = "100%" border = "1">
    <tr>
        <th>Aluno</th>
        <th colspan="2"> Disciplinas</th>
    </tr>
    <tr>
        <td>Alex</td>
        <td>Html</td>
        <td>JavasCript</td>
    </tr>
   </table>
  <details>
    <summary>Mostrar Código HTML</summary>
    
    
  ```html 
  <table widht = "100%" border = "1">
    <tr>
        <th>Aluno</th>
        <th colspan="2"> Disciplinas</th>
    </tr>
    <tr>
        <td>Alex</td>
        <td>Html</td>
        <td>JavasCript</td>
    </tr>
   </table>
  ```
 </details>

 ## Tabela com Rolspan 

 <table width = "100%" border ="1">
   <tr>
     <th>Aluno:</th>
     <td>Alex</td>
   </tr>
   <tr>
     <th rowspan ="2">Disciplinas:</th>
     <td>HTML</td>
   </tr>
   <tr>
     <td>JavaScript</td>
   </tr>
 </table>
 <details>
    <summary>Mostrar Código HTML</summary>
    
    
  ```html 
  <table width = "100%" border ="1">
   <tr>
     <th>Aluno:</th>
     <td>Alex</td>
   </tr>
   <tr>
     <th rowspan ="2">Disciplinas:</th>
     <td>HTML</td>
   </tr>
   <tr>
     <td>JavaScript</td>
   </tr>
 </table>
  ```
 </details>

