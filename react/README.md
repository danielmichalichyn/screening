# Screening - React / NextJS

## Objetivo
Criar uma interface que consuma um JSON de uma API e exiba as informações como um menu ordenado, respeitando as relações de parentesco.

## Descrição da Tarefa
Você receberá um objeto JSON contendo uma lista de locais. Cada local possui um `id`, `nome`, `descrição` e um campo opcional `parent`. O campo `parent` indica o ID do local pai, se existir. Sua tarefa é criar uma interface web que busque esses dados de um endpoint de API e os exiba em um formato de menu hierárquico, mostrando as suas relações.

## Requisitos
1. **Buscar Dados da API**:
   - Você pode simplesmente colar o JSON abaixo em uma constante de seu código e "mockar" a resposta de uma API a partir dessa variável.

2. **Design da Interface**:
   - Exibir os locais em um menu ordenado e aninhado. Locais sem "parent" devem ser mostrados no nível superior, e seus filhos devem ser aninhados abaixo deles, devidamente indentados.
   - Usar um design simples e limpo para a interface. Você pode usar React, NextJS ou JavaScript puro para este desafio.

3. **Funcionalidade**:
   - Ao clicar no nome de um local no menu, exibir a descrição correspondente em um canvas dedicado no centro da tela.
   - Implementar uma indicação visual (como um ícone ou seta) para mostrar o estado expansível/colapsável para locais com filhos.
   - Implementar qual item do menu está atualmente selecionado.

4. **Qualidade do Código**:
   - Escrever código limpo, de fácil manutenção e bem documentado.
   - Garantir que a solução seja responsiva e funcione em diferentes dispositivos e tamanhos de tela.

## Pontos Extras
- Implementar funcionalidade de busca para filtrar locais por nome.
- Usar TypeScript para segurança de tipos.
- Implementar testes unitários para os principais componentes e lógica.

## Entregáveis
1. Um repositório contendo todo o código-fonte da sua implementação.
2. Um arquivo `README.md` explicando como configurar e executar o projeto, bem como qualquer outra informação relevante.

## Exemplo de JSON
```json
{
    "locations":[
        {
            "name":"Location 1",
            "description":"Location 1 - Description",
            "id":1,
            "parent": null
        },
        {
            "name":"Location 2",
            "description":"Location 2 - Description",
            "id":2,
            "parent": null
        },
        {
            "name":"Location 1.1",
            "description":"Location 1.1 - Description",
            "id":3,
            "parent":1
        },
        {
            "name":"Location 2.1",
            "description":"Location 2.1 - Description",
            "id":4,
            "parent":2
        },
        {
            "name":"Location 2.2",
            "description":"Location 2.2 - Description",
            "id":5,
            "parent":2
        },
        {
            "name":"Location 2.1.1",
            "description":"Location 2.1.1 - Description",
            "id":6,
            "parent":4
        },
        {
            "name":"Location 1.2",
            "description":"Location 1.2 - Description",
            "id":7,
            "parent":1
        }
    ]
}
