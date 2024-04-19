📦 Laravel Pagination with Bootstrap
Problema
Em projetos Laravel, a paginação é estilizada com Tailwind CSS, o que pode ser problemático quando se deseja utilizar outro framework CSS, como Bootstrap.

Solução
Este pacote oferece uma solução abrangente para este problema. Ele permite que os desenvolvedores utilizem a funcionalidade de paginação do Laravel enquanto aplicam facilmente estilos do Bootstrap.

Recursos
🛠️ Fácil integração com projetos Laravel existentes.
🎨 Personalização flexível para atender às necessidades específicas de estilo.
Como Usar
Baixe o arquivo e coloque-o dentro da sua view.

Na Controller:

public function receberDadosDoBanco(){ $dados = Models::paginate(5); return view('sua.view', ['dados' => $dados]); }

Na View:

{{ $dados->links('pagination') }}
