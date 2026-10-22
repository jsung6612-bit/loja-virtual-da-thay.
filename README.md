# Loja Virtual da Thay 🎀

Projeto inicial de loja virtual em Next.js com identidade visual rosa e preto, estilo luxo, responsiva para celular e computador. A vitrine começa vazia de propósito: os produtos serão cadastrados mais tarde.

## O que está preparado
- Página inicial com identidade visual rosa/preto e estilo elegante.
- Categorias para moda, beleza, acessórios, eletrônicos, casa e novidades.
- Área de catálogo com busca e filtro, preparada para ler produtos do Supabase.
- Área visual de sacola/carrinho para demonstração da experiência.
- Página `/admin` com o roteiro de preparação do painel administrativo.
- Esquema inicial do banco de dados para produtos e pedidos, sem produtos de exemplo.

## Importante: ainda não está pronta para vendas reais
O painel administrativo é, neste momento, uma página de configuração — ainda não tem login nem cadastro funcional de produtos. O carrinho é demonstrativo e o checkout/pagamentos não estão ativados nesta versão. Não divulgue o site como loja pronta para receber pedidos e não coloque chaves secretas no navegador.

## Como testar no computador
1. Instale Node.js LTS.
2. Extraia o ZIP e abra a pasta `loja-virtual-da-thay` no terminal.
3. Execute `npm install`.
4. Copie `.env.example` para `.env.local`.
5. Execute `npm run dev` e abra `http://localhost:3000`.

Sem Supabase configurado, a vitrine mostrará a mensagem de que os produtos serão adicionados depois. O banco pode ser preparado quando você estiver pronta para cadastrar itens.

## Publicar gratuitamente (quando estiver pronta)
Uma opção comum é usar um plano gratuito de hospedagem compatível com Next.js, como Vercel, e um banco Supabase. Os limites e condições dos planos podem mudar. Para publicar com catálogo dinâmico:
1. Crie um projeto Supabase e execute `supabase/schema.sql` no SQL Editor.
2. Configure as variáveis de ambiente do projeto no ambiente de hospedagem.
3. Antes de abrir o cadastro de produtos, implemente autenticação de administrador e autorização no servidor.
4. Configure domínio gratuito fornecido pela hospedagem, se disponível.
5. Só depois conecte checkout, pagamentos, frete, controle seguro de estoque e notificações.

## Próximas etapas de desenvolvimento
1. Implementar login administrativo protegido e recuperação de acesso.
2. Criar operações de servidor seguras para cadastrar, editar, ocultar e excluir produtos.
3. Adicionar upload de fotos e gestão real de estoque.
4. Concluir checkout, frete e integração de pagamentos com webhooks validados.
5. Preparar política de privacidade, termos, trocas/devoluções e informações de contato.
6. Testar em celular e computador antes de divulgar.

Para menores de 18 anos, peça ajuda a um responsável para criar/configurar contas de hospedagem, banco de dados e serviços de pagamento que tenham exigência de idade. Nunca compartilhe senhas, tokens ou chaves secretas no chat.
