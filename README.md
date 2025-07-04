# Como Editar o Site da Conteal

Este site é composto por arquivos HTML, CSS e JavaScript, o que facilita a edição do conteúdo e a personalização do design. Você não precisa de nenhum software especial, apenas um editor de texto.

## Estrutura de Arquivos

-   `index.html`: Página inicial do site.
-   `servicos.html`: Página com a descrição dos serviços.
-   `contato.html`: Página com as informações de contato.
-   `css/style.css`: Arquivo CSS com estilos gerais do site.
-   `css/segments.css`: Arquivo CSS com estilos específicos para as seções de segmentos.

## Como Editar o Conteúdo

Para editar o conteúdo de qualquer página, siga os passos abaixo:

1.  **Abra o Arquivo:** Use um editor de texto (como Bloco de Notas no Windows, TextEdit no Mac, ou editores mais avançados como VS Code, Sublime Text, Notepad++) para abrir o arquivo HTML que deseja editar (ex: `index.html`).

2.  **Localize o Texto:** Procure pelo texto que você deseja alterar. O conteúdo visível do site estará dentro de tags HTML como `<p>` (parágrafo), `<h1>` a `<h6>` (títulos), `<span>`, `<a>` (links), etc.

    *   **Exemplo:** Para alterar o slogan na página inicial, procure por `<h1>Conteal: Segurança e Tecnologia</h1>` e edite o texto entre as tags `<h1>` e `</h1>`.

3.  **Edite o Conteúdo:** Altere o texto conforme necessário. Tenha cuidado para não apagar as tags HTML (como `<`, `>`, `/`), pois elas definem a estrutura da página.

    *   **Para adicionar um novo serviço em `servicos.html`:** Você pode copiar e colar um bloco `div` existente com a classe `product-item` e modificar o conteúdo. Lembre-se de que as imagens de exemplo (`https://via.placeholder.com/`) podem ser substituídas por suas próprias imagens.
        ```html
        <div class="product-item">
            <div class="product-image" style="background-image: url(\'https://via.placeholder.com/400x200/CCCCCC/FFFFFF?text=Novo+Servico\');"></div>
            <div class="product-content">
                <h4>Nome do Novo Serviço</h4>
                <p>Descrição detalhada do seu novo serviço.</p>
                <ul class="product-features">
                    <li><i class="fas fa-check"></i> Característica 1</li>
                    <li><i class="fas fa-check"></i> Característica 2</li>
                </ul>
                <a href="#" class="product-btn">Saiba Mais</a>
            </div>
        </div>
        ```

    *   **Para alterar o número do WhatsApp:** Edite o link `href` no arquivo `index.html` e `contato.html`. Procure por `https://wa.me/5551993320242` e substitua o número `5551993320242` pelo novo número (incluindo o código do país e DDD, sem espaços ou caracteres especiais).

    *   **Para alterar as opções AGRO, INDÚSTRIA, COMÉRCIO na página inicial:** Edite o texto dentro das tags `<h3>` e `<p>` dentro das `div`s com a classe `segment-card` no arquivo `index.html`.

4.  **Salve o Arquivo:** Salve as alterações no arquivo. Certifique-se de salvar com a mesma extensão `.html`.

5.  **Visualize as Alterações:** Para ver suas alterações, basta abrir o arquivo HTML no seu navegador. Se o site já estiver online no GitHub Pages, você precisará fazer o commit e push das alterações para o repositório (conforme explicado na próxima seção) para que elas apareçam online.

## Edição de Estilos (CSS)

Os estilos (cores, fontes, layout) estão definidos nos arquivos `css/style.css` e `css/segments.css`. Se você tiver conhecimento de CSS, pode modificar esses estilos para personalizar a aparência do site. Por exemplo, para mudar a cor de fundo do cabeçalho, procure por `background-color: #333;` dentro do bloco `header` no arquivo `css/style.css`.

## Próximos Passos: Publicando no GitHub Pages

Depois de fazer suas edições, o próximo passo é publicar o site no GitHub Pages. Você precisará de uma conta no GitHub e de um cliente Git instalado no seu computador. As instruções detalhadas para isso serão fornecidas separadamente.

