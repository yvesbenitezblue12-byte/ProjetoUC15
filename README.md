Projeto integrador  – Documentação técnica
Responsável: (Yves Daniel Manso Benitez)
Nome do sistema: (Cadastro de Filmes)
Versão: (1.0))
Apresentação
[Esse é um sistema de banco de dados para Cadastro de filmes,consultas,exclusao, aonde possui 3 tipos de usuarios: administrador, operador, usuario cada um com suas permissoes.
]
Descrição do projeto e usuários
Neste espaço, descreva, agora de maneira mais técnica, o que conterá o seu sistema: as funcionalidades, as condições e a estrutura de todo esse sistema. É importante descrever as funcionalidades de acordo com as telas e permissões de usuários (caso existam).
[O sistema é uma aplicação para gerenciamento de uma Locadora de Filmes, cujo objetivo é controlar:
    • Filmes Cadastrados
    • Consultar Filmes
    • Excluir Filmes
    • Permissoes dos 3 tipos de usuarios
    • Controle de Permissões de acesso
Os usuários e suas permissões:
    • Administrador – Acesso a todos os cadastros,consultas e exclusao
    • Operador – Cadastrar e Consultar
    • Usuario - Consultar
]
Requisitos funcionais
Aqui, descreva os requisitos funcionais do projeto, respeitando a estrutura, numeração e funcionalidade para listar estes requisitos. Lembre-se de que um requisito funcional é uma ação que o sistema realiza, geralmente tendo interação com os usuários já listados.
[RF01 – Gerenciar clientes
O sistema deve permitir o cadastro, consulta, atualização e exclusão de filmes.

RF02 – Validar Alterações
O sistema deve permitir que os dados sejam enviados para o banco de dados

RF03 – Gerenciar funcionários
O sistema deve permitir cadastro,consulta e exclusão dos dados dos dilmes (apenas perfil administrador).

RF04 – Gerenciar consultas
O sistema deve permitir o acesso de consultas para todos os usuarios.

RF05 – Exibir lista
O sistema deve exibir a lista dos filmes cadastrados.

RF06 – Remover filmes 
Ao excluir um filme, ele tambem precisa ser excluido automaticamente no banco de dados.

RF07 – Manter consultas mesmo após a exclusão do funcionário
Ao excluir um filme, as consultas previamente registradas devem permanecer, mas com o campo id_funcionario definido como NULL (regra ON DELETE SET NULL).



RF08 – Consultar registros com filtros
O sistema deve permitir buscar: Clientes por nome, CPF, e-mail,funcionários por cargo,consultas por data, cliente, funcionário ou status, pagamentos por forma de pagamento e data.

RF09 – Controlar usuários e permissões
O sistema deve permitir dois níveis de acesso: Administrador: acesso total
Operador: acesso apenas para cadastro e consulta
Usuario: Consulta
Requisitos não funcionais
Similar ao campo anterior, é neste espaço que você inserirá os requisitos não funcionais do projeto. Respeite a estrutura, numeração e funcionalidade para listar estes requisitos. Vale ressaltar que um requisito não funcional é aquele que não está diretamente relacionado a uma funcionalidade do sistema, mas sim foca em aspectos de usabilidade, manutenção e desempenho, nos quais não existe uma interação do usuário.
[RNF01 – Segurança no acesso ao banco 
As permissões de usuários devem ser controladas diretamente no banco utilizando GRANT e REVOKE, restringindo ações por perfil.

RNF02 – Integridade referencial
O sistema deve garantir a integridade dos dados por meio das constraints: chaves primárias, chaves estrangeiras, regras ON DELETE / ON UPDATE

RNF03 – Disponibilidade e consistência dos dados
O banco deve manter consistência lógica para evitar registros órfãos ou inconsistentes.

RNF04 – Confiabilidade no armazenamento
Os dados devem ser armazenados em um sistema relacional (MySQL) garantindo persistência e confiabilidade.

RNF05 – Padronização das informações
Campos como forma de pagamento e status de consultas devem seguir padrões estabelecidos

RNF06 – Desempenho nas consultas
Índices, chaves primárias e relacionamentos devem garantir performance adequada para consultas frequentes.

RNF07 – Auditabilidade
Os registros devem conter timestamps automáticos que permitam auditoria e rastreamento das operações.

RNF08 – Usabilidade
O sistema deve apresentar uma interface clara e objetiva, onde: Administradores consigam gerenciar cadastros,consultas e excluir filmes.

Observações técnicas
Utilize este campo para trazer observações acerca do seu sistema, questões relacionadas às tecnologias que serão usadas (como a linguagem de programação Java e o banco de dados MySQL), algum sistema de backup utilizando o banco de dados ou alguma regra de negócio específica de acordo com a necessidade do cliente ou dos usuários.
[O modelo atende completamente o fluxo operacional de uma Locadora de Filmes o banco foi projetado para a tecnologia Mysql Server, para garantir segurança dos dados deve executar backups diariamente]
