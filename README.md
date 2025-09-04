# Eng_Software_02.2025
Estudo Dirigido - Engenharia de Software

## - [1. Introdução](#1-introdução)
>> Descrever a necessidade de um sistema nessa área em até 2 ou 3 parágrafos.

<!--  Função/Persona: Você é um consultor especialista em sistemas de gestão para a   indústria de mineração. Sua tarefa é redigir a introdução de uma proposta de projeto para o desenvolvimento de um Sistema de Gerenciamento de Operações de Mineração (SGOM). 
Objetivo: Elaborar uma introdução concisa, em 2 ou 3 parágrafos, que descreva a necessidade crítica de um sistema de informação integrado para uma empresa de mineração com operações complexas. A introdução deve contextualizar o leitor sobre os desafios do setor e justificar a importância da solução proposta. 
Instruções: No primeiro parágrafo, aborde a complexidade da operação, destacando como a diversidade de dados gerados (operacionais, ambientais, regulatórios) impõe desafios significativos à gestão, eficiência e conformidade. No parágrafo seguinte, justifique a necessidade de um sistema integrado como solução estratégica. Enfatize os ganhos em rastreabilidade, segurança da informação e a capacidade de correlacionar dados distintos (ex: produção vs. clima) para otimizar as operações e a tomada de decisão. Lembrando de utilizar como base o arquivo de Descrição_Empresa, que foi passado anteriormente. --> 
 
As operações de mineração apresentam uma complexidade única, resultado da diversidade de processos envolvidos e da variedade de dados que precisam ser monitorados e controlados. No caso desta empresa, que possui autorização para explorar ouro, casiterita, dolomito e zinco em diferentes jazidas, o volume de informações geradas é expressivo: registros de produção diária, qualidade dos lotes, controle ambiental (fauna, flora e áreas de preservação), dados climáticos provenientes de estação meteorológica, além de documentos regulatórios e de conformidade legal. A ausência de uma gestão integrada desses elementos cria desafios significativos para assegurar eficiência operacional, conformidade normativa e rastreabilidade em toda a cadeia produtiva.

Diante desse cenário, a implementação de um Sistema de Gerenciamento de Operações de Mineração (SGOM) surge como uma solução estratégica para unificar e correlacionar informações críticas. Um sistema integrado permitirá consolidar registros operacionais, ambientais e administrativos em uma única plataforma, assegurando maior segurança da informação e facilitando auditorias internas e externas. Além disso, a capacidade de relacionar dados de produção com variáveis climáticas e ambientais proporcionará análises preditivas e decisões mais assertivas, promovendo ganhos em eficiência, redução de riscos e otimização de recursos, fortalecendo assim a competitividade e a sustentabilidade da mineradora.

## - [2. Descrição](#2-descrição)
  - [2.1. Requisitos.](#21-requisitos)
>> Colocar aqui a lista acima!

<!-- 
    Prompt: Função/Persona: Você é um Analista de Requisitos Sênior. Sua principal habilidade é traduzir descrições de processos de negócio em requisitos de sistema claros, organizados e acionáveis.

Objetivo: Com base na descrição detalhada da empresa de mineração fornecida anteriormente, gerar uma lista completa de requisitos funcionais e não funcionais para o Sistema de Gerenciamento de Operações de Mineração (SGOM). O resultado deve ser um documento único, formatado em Markdown, pronto para ser usado pela equipe de desenvolvimento e gestão do projeto.

Instruções de Formatação e Conteúdo:

Formato Geral: O output deve ser inteiramente em Markdown.

Título Principal: Comece o documento com um título de primeiro nível, como # Requisitos do Sistema de Gerenciamento de Operações de Mineração (SGOM).

Estrutura em Módulos: Agrupe os requisitos em módulos lógicos para melhor organização. Utilize títulos de segundo nível (##) para cada módulo. Sugestões de módulos:

Gestão de Áreas e Produção

Controle de Atividades e Lavra

Gestão de Qualidade e Certificação

Logística, Expedição e Subprodutos

Monitoramento Ambiental e Sustentabilidade

Administração (Funcionários, Veículos e Equipamentos)

Gestão de Documentos e Dados Geoespaciais

Requisitos Não Funcionais

Lista de Requisitos: Dentro de cada módulo, liste os requisitos individuais utilizando a sintaxe de checklist do Markdown (- [ ]). Cada item deve descrever uma funcionalidade específica derivada do cenário.

Exemplo: - [ ] Permitir o cadastro de áreas com coordenadas delimitadoras, definindo seu tipo (ex: jazida, reserva legal, pátio).

Clareza e Rastreabilidade: Cada requisito deve ser conciso e corresponder diretamente a uma ou mais das 30 descrições fornecidas, garantindo que todas as necessidades do negócio sejam cobertas.

Requisitos Não Funcionais: Crie uma seção específica para requisitos que descrevem como o sistema deve operar, como armazenamento de arquivos, integração de dados e segurança.

Exemplo: - [ ] O sistema deve suportar o upload, armazenamento e visualização de arquivos no formato PDF.
-->

# Requisitos do Sistema de Gerenciamento de Operações de Mineração (SGOM)

| ID     | Módulo                                   | Requisito |
|--------|------------------------------------------|-----------|
| RF001  | Gestão de Áreas e Produção              | Permitir o cadastro de áreas com coordenadas delimitadoras, definindo seu tipo (jazida, reserva legal, pátio, área administrativa). |
| RF002  | Gestão de Áreas e Produção              | Registrar a licença de exploração da área, incluindo data de início e data final. |
| RF003  | Gestão de Áreas e Produção              | Cadastrar múltiplas jazidas, informando os minerais exploráveis (ouro, casiterita, dolomito, zinco). |
| RF004  | Gestão de Áreas e Produção              | Registrar produção diária de cada área, incluindo quantidade, data e tipo de mineral. |
| RF005  | Gestão de Áreas e Produção              | Controlar registros de valor de mercado do minério na data da produção. |
| RF006  | Gestão de Áreas e Produção              | Relacionar dados climáticos coletados com a produção de cada área. |
| RF007  | Gestão de Áreas e Produção              | Registrar produção de areia de cascalho como subproduto da mineração. |
| RF008  | Controle de Atividades e Lavra          | Permitir o cadastro de atividades de lavra (prospecção, avaliação de amostras, preparo de área, extração, filtragem, pesagem, testes de qualidade, registro de produção, expedição). |
| RF009  | Controle de Atividades e Lavra          | Registrar detalhes de cada atividade: código, responsável, data/hora de início e fim, área de execução. |
| RF010  | Controle de Atividades e Lavra          | Associar cada lote extraído a um identificador único, vinculado à atividade de extração. |
| RF011  | Controle de Atividades e Lavra          | Registrar informações detalhadas das operações de lavra: local, data, hora, responsável e descrição da operação. |
| RF012  | Controle de Atividades e Lavra          | Registrar a expedição final, incluindo o armazenamento em cofre e identificação do responsável. |
| RF013  | Gestão de Qualidade e Certificação      | Registrar testes de qualidade de cada lote, contendo código da área, responsável, data, volume e peso. |
| RF014  | Gestão de Qualidade e Certificação      | Definir e aplicar níveis de pureza dos minerais conforme tabela de padrões. |
| RF015  | Gestão de Qualidade e Certificação      | Emitir selo de pureza quando o lote atingir o padrão exigido. |
| RF016  | Gestão de Qualidade e Certificação      | Permitir análise de qualidade realizada por especialistas e por visão computacional. |
| RF017  | Gestão de Qualidade e Certificação      | Emitir certificados de origem e de nível de pureza dos materiais comercializados. |
| RF018  | Logística, Expedição e Subprodutos      | Cadastrar os tipos de equipamentos específicos para extração e transporte de cada mineral. |
| RF019  | Logística, Expedição e Subprodutos      | Registrar movimentação de veículos e equipamentos durante as operações. |
| RF020  | Logística, Expedição e Subprodutos      | Gerenciar subprodutos da mineração, como areia e cascalho, incluindo volume de produção e destinação. |
| RF021  | Logística, Expedição e Subprodutos      | Controlar registros de expedição, vinculando lotes e responsáveis. |
| RF022  | Monitoramento Ambiental e Sustentabilidade | Cadastrar e monitorar fauna presente na região (espécies de animais). |
| RF023  | Monitoramento Ambiental e Sustentabilidade | Cadastrar e monitorar árvores dentro e ao redor da propriedade. |
| RF024  | Monitoramento Ambiental e Sustentabilidade | Registrar e armazenar mapas (altimétrico, geomorfológico, hídrico, topográfico, de áreas de extração, preservação, pátios e administrativos). |
| RF025  | Monitoramento Ambiental e Sustentabilidade | Registrar e acompanhar projetos de reflorestamento ou plantio em áreas desativadas. |
| RF026  | Monitoramento Ambiental e Sustentabilidade | Integrar dados da estação meteorológica automática (pluviômetro e outros sensores). |
| RF027  | Monitoramento Ambiental e Sustentabilidade | Relacionar informações ambientais com operações e produção. |
| RF028  | Administração (Funcionários e Equipamentos) | Cadastrar funcionários com dados pessoais, função, engenheiros responsáveis e alocação por área. |
| RF029  | Administração (Funcionários e Equipamentos) | Cadastrar veículos e maquinário, relacionando com responsáveis e engenheiros. |
| RF030  | Administração (Funcionários e Equipamentos) | Controlar permissões de acesso dos usuários ao sistema conforme função e responsabilidade. |
| RF031  | Gestão de Documentos e Dados Geoespaciais | Permitir o upload, armazenamento e visualização de documentos em PDF (laudos, relatórios, alvarás, concessões, portarias). |
| RF032  | Gestão de Documentos e Dados Geoespaciais | Organizar documentos por tipo, data, responsável e área vinculada. |
| RF033  | Gestão de Documentos e Dados Geoespaciais | Permitir armazenamento e visualização de imagens e vídeos de câmeras de monitoramento. |
| RF034  | Gestão de Documentos e Dados Geoespaciais | Integrar dados geoespaciais (mapas) ao cadastro de áreas, possibilitando visualização e análise. |
| RNF001 | Requisitos Não Funcionais                | O sistema deve suportar upload, armazenamento e visualização de arquivos PDF. |
| RNF002 | Requisitos Não Funcionais                | O sistema deve ser capaz de armazenar grandes volumes de dados (produção, ambientais, documentos, imagens). |
| RNF003 | Requisitos Não Funcionais                | O sistema deve assegurar rastreabilidade e integridade das informações registradas. |
| RNF004 | Requisitos Não Funcionais                | O sistema deve garantir segurança da informação, com autenticação de usuários e trilha de auditoria. |
| RNF005 | Requisitos Não Funcionais                | O sistema deve permitir integração com estação meteorológica automática. |
| RNF006 | Requisitos Não Funcionais                | O sistema deve suportar relacionamentos cruzados entre diferentes módulos (ex.: produção x clima). |
| RNF007 | Requisitos Não Funcionais                | O sistema deve possibilitar consultas e relatórios customizáveis. |
| RNF008 | Requisitos Não Funcionais                | O sistema deve ser escalável para atender futuras ampliações da área de mineração ou novos tipos de minerais. |
| RNF009 | Requisitos Não Funcionais                | O sistema deve manter compatibilidade com auditorias, permitindo exportação de registros em formatos padrão. |
| RNF010 | Requisitos Não Funcionais                | O sistema deve permitir integração futura com ferramentas de análise de dados e inteligência artificial. |

##  - [2.2. Funcionais e não-funcionais](#22-funcionais-e-não-funcionais)
>> via prompt, separar os requisitos por tipo (funcional e não funcional), colocar aqui em forma de tabela markdown
<!-- 
Objetivo: Pegar uma lista mista de requisitos de sistema (já elaborada) para o SGOM e classificá-la de forma clara e distinta em duas categorias: Requisitos Funcionais e Requisitos Não Funcionais. O resultado final deve ser um documento Markdown limpo e bem estruturado.

Contexto de Entrada: O prompt receberá como entrada uma lista de requisitos do SGOM, previamente gerados e possivelmente agrupados por módulos.

Instruções de Execução:

Estrutura do Documento: Crie um documento Markdown com dois títulos principais de segundo nível (##):

## Requisitos Funcionais

## Requisitos Não Funcionais

Critérios de Classificação:

Requisitos Funcionais: São as funcionalidades que o sistema deve fazer. Descrevem ações, interações do usuário ou processos de negócio. (Ex: "O sistema deve permitir o cadastro de funcionários", "O sistema deve registrar a produção diária de minério").

Requisitos Não Funcionais: São as qualidades, restrições e características de como o sistema deve ser ou operar. Descrevem atributos como desempenho, segurança, usabilidade ou compatibilidade. (Ex: "O sistema deve suportar o armazenamento de arquivos PDF", "O sistema deve garantir a segurança dos dados de expedição", "A interface deve ser responsiva").

Processo:

Analise CADA item da lista de requisitos fornecida.

Mova cada requisito para baixo do título correspondente (Funcional ou Não Funcional).

Mantenha o texto original e o formato de checklist (- [ ]) para cada requisito. Não é necessário reescrevê-los, apenas realocá-los.

Resultado Esperado: Um único documento Markdown contendo todos os requisitos originais, mas agora perfeitamente separados nas duas categorias definidas, facilitando o planejamento técnico do projeto.
-->

# Requisitos do Sistema de Gerenciamento de Operações de Mineração (SGOM)

| ID     | Tipo                 | Descrição |
|--------|----------------------|-----------|
| RF001  | Funcional            | Permitir o cadastro de áreas com coordenadas delimitadoras, definindo seu tipo (jazida, reserva legal, pátio, área administrativa). |
| RF002  | Funcional            | Registrar a licença de exploração da área, incluindo data de início e data final. |
| RF003  | Funcional            | Cadastrar múltiplas jazidas, informando os minerais exploráveis (ouro, casiterita, dolomito, zinco). |
| RF004  | Funcional            | Registrar produção diária de cada área, incluindo quantidade, data e tipo de mineral. |
| RF005  | Funcional            | Controlar registros de valor de mercado do minério na data da produção. |
| RF006  | Funcional            | Relacionar dados climáticos coletados com a produção de cada área. |
| RF007  | Funcional            | Registrar produção de areia de cascalho como subproduto da mineração. |
| RF008  | Funcional            | Permitir o cadastro de atividades de lavra (prospecção, avaliação de amostras, preparo de área, extração, filtragem, pesagem, testes de qualidade, registro de produção, expedição). |
| RF009  | Funcional            | Registrar detalhes de cada atividade: código, responsável, data/hora de início e fim, área de execução. |
| RF010  | Funcional            | Associar cada lote extraído a um identificador único, vinculado à atividade de extração. |
| RF011  | Funcional            | Registrar informações detalhadas das operações de lavra: local, data, hora, responsável e descrição da operação. |
| RF012  | Funcional            | Registrar a expedição final, incluindo o armazenamento em cofre e identificação do responsável. |
| RF013  | Funcional            | Registrar testes de qualidade de cada lote, contendo código da área, responsável, data, volume e peso. |
| RF014  | Funcional            | Definir e aplicar níveis de pureza dos minerais conforme tabela de padrões. |
| RF015  | Funcional            | Emitir selo de pureza quando o lote atingir o padrão exigido. |
| RF016  | Funcional            | Permitir análise de qualidade realizada por especialistas e por visão computacional. |
| RF017  | Funcional            | Emitir certificados de origem e de nível de pureza dos materiais comercializados. |
| RF018  | Funcional            | Cadastrar os tipos de equipamentos específicos para extração e transporte de cada mineral. |
| RF019  | Funcional            | Registrar movimentação de veículos e equipamentos durante as operações. |
| RF020  | Funcional            | Gerenciar subprodutos da mineração, como areia e cascalho, incluindo volume de produção e destinação. |
| RF021  | Funcional            | Controlar registros de expedição, vinculando lotes e responsáveis. |
| RF022  | Funcional            | Cadastrar e monitorar fauna presente na região (espécies de animais). |
| RF023  | Funcional            | Cadastrar e monitorar árvores dentro e ao redor da propriedade. |
| RF024  | Funcional            | Registrar e armazenar mapas (altimétrico, geomorfológico, hídrico, topográfico, de áreas de extração, preservação, pátios e administrativos). |
| RF025  | Funcional            | Registrar e acompanhar projetos de reflorestamento ou plantio em áreas desativadas. |
| RF026  | Funcional            | Integrar dados da estação meteorológica automática (pluviômetro e outros sensores). |
| RF027  | Funcional            | Relacionar informações ambientais com operações e produção. |
| RF028  | Funcional            | Cadastrar funcionários com dados pessoais, função, engenheiros responsáveis e alocação por área. |
| RF029  | Funcional            | Cadastrar veículos e maquinário, relacionando com responsáveis e engenheiros. |
| RF030  | Funcional            | Controlar permissões de acesso dos usuários ao sistema conforme função e responsabilidade. |
| RF031  | Funcional            | Permitir o upload, armazenamento e visualização de documentos em PDF (laudos, relatórios, alvarás, concessões, portarias). |
| RF032  | Funcional            | Organizar documentos por tipo, data, responsável e área vinculada. |
| RF033  | Funcional            | Permitir armazenamento e visualização de imagens e vídeos de câmeras de monitoramento. |
| RF034  | Funcional            | Integrar dados geoespaciais (mapas) ao cadastro de áreas, possibilitando visualização e análise. |
| RNF001 | Não Funcional        | O sistema deve suportar upload, armazenamento e visualização de arquivos PDF. |
| RNF002 | Não Funcional        | O sistema deve ser capaz de armazenar grandes volumes de dados (produção, ambientais, documentos, imagens). |
| RNF003 | Não Funcional        | O sistema deve assegurar rastreabilidade e integridade das informações registradas. |
| RNF004 | Não Funcional        | O sistema deve garantir segurança da informação, com autenticação de usuários e trilha de auditoria. |
| RNF005 | Não Funcional        | O sistema deve permitir integração com estação meteorológica automática. |
| RNF006 | Não Funcional        | O sistema deve suportar relacionamentos cruzados entre diferentes módulos (ex.: produção x clima). |
| RNF007 | Não Funcional        | O sistema deve possibilitar consultas e relatórios customizáveis. |
| RNF008 | Não Funcional        | O sistema deve ser escalável para atender futuras ampliações da área de mineração ou novos tipos de minerais. |
| RNF009 | Não Funcional        | O sistema deve manter compatibilidade com auditorias, permitindo exportação de registros em formatos padrão. |
| RNF010 | Não Funcional        | O sistema deve permitir integração futura com ferramentas de análise de dados e inteligência artificial. |

<!-- ## - [3. Diagramas](#3-diagramas)
  - [3.1. Diagrama de classe](#31-diagrama-de-classe)
 Crie um prompt para o diagrama de classe usando Markdown e Mermaid.
-->
<!-- 
Função/Persona: Você é um Arquiteto de Software Sênior, especializado em modelagem de dados e design de sistemas. Sua tarefa é traduzir um complexo cenário de negócios em um Diagrama de Classe UML claro e preciso.

Objetivo: Com base na descrição detalhada da empresa de mineração, criar um Diagrama de Classe abrangente utilizando a sintaxe Mermaid dentro de um bloco de código Markdown. O diagrama deve modelar as principais entidades, seus atributos, métodos e os relacionamentos entre elas para o Sistema de Gerenciamento de Operações de Mineração (SGOM).

Instruções de Execução:

Formato de Saída: O resultado deve ser um único bloco de código Markdown formatado para Mermaid. Inicie o bloco com ```mermaid e termine com ```.

Identificação de Classes: Analise a descrição da empresa e identifique as principais entidades que devem se tornar classes. Algumas sugestões são: Empresa, Area, Jazida, Mineral, AtividadeLavra, Funcionario, Equipamento, LoteProducao, TesteQualidade, Documento, Mapa, Animal, Arvore, EstacaoMeteorologica, DadoClimatico, etc.

Definição de Atributos: Para cada classe, adicione os atributos relevantes com seus tipos de dados (ex: string, int, float, date, datetime).

Exemplo:

class LoteProducao {
    +int idLote
    +date dataExtracao
    +float quantidade
    +string tipoMineral
}

Definição de Métodos: Inclua métodos que representem as principais operações que cada classe pode realizar. Use parênteses () para indicar um método.

Exemplo:

class TesteQualidade {
    +string responsavel
    +date data
    +float volume
    +float peso
    +realizarTeste()
    +gerarCertificado()
}

Modelagem de Relacionamentos e Cardinalidades: Conecte as classes usando as setas apropriadas do Mermaid para representar herança, composição, agregação e associação. Adicione as cardinalidades para especificar as relações.

Composição (um contém muitos): Empresa "1" *-- "3" Jazida (A empresa é composta por 3 jazidas)

Associação (um se relaciona com muitos): Funcionario "1" -- "*" AtividadeLavra (Um funcionário pode ser responsável por várias atividades)

Agregação (um tem um): LoteProducao "1" o-- "1" TesteQualidade (Um lote tem um teste de qualidade)

Herança (é um tipo de): Engenheiro --|> Funcionario (Engenheiro é um tipo de Funcionário)

Diagrama Completo: Combine todas as classes e relacionamentos em um único diagrama classDiagram, garantindo que a lógica do negócio descrita no cenário seja representada de forma coesa e correta.
-->

classDiagram

class Empresa {
  +id: int
  +nome: string
  +cnpj: string
  +endereco: string
  +criarArea()
  +registrarDocumento()
  +emitirRelatorios()
  +correlacionarProducaoClima()
}

class LicencaExploracao {
  +id: int
  +numeroOutorga: string
  +dataInicio: date
  +dataFim: date
  +orgaoEmissor: string
  +estaVigente(): bool
}

class Area {
  +id: int
  +nome: string
  +tipo: string
  +descricao: string
  +registrarProducao()
  +iniciarAtividade()
  +finalizarAtividade()
  +anexarMapa()
}

class Jazida {
  +metodoLavra: string
  +observacoes: string
}

class ReservaLegal {
  +nivelProtecao: string
  +restricoes: string
}

class Patio {
  +finalidade: string
  +capacidadeEstoque: float
}

class Administrativa {
  +departamento: string
}

class Coordenada {
  +id: int
  +latitude: float
  +longitude: float
  +ordemVertice: int
}

class Mineral {
  +id: int
  +nome: string
  +unidadeMedida: string
}

class AtividadeLavra {
  +id: int
  +codigo: string
  +tipo: string
  +inicio: datetime
  +fim: datetime
  +detalhes: string
  +iniciar()
  +encerrar()
}

class LoteProducao {
  +idLote: int
  +dataExtracao: date
  +quantidade: float
  +peso: float
  +valorMinerioData: float
  +registrar()
  +vincularTesteQualidade()
  +prepararExpedicao()
}

class TesteQualidade {
  +id: int
  +data: date
  +volume: float
  +peso: float
  +responsavel: string
  +realizarTeste()
  +calcularPureza()
  +gerarLaudoPDF()
}

class NivelPureza {
  +id: int
  +nomeNivel: string
  +purezaMinima: float
  +purezaMaxima: float
  +descricao: string
}

class SeloPureza {
  +id: int
  +codigoSelo: string
  +dataEmissao: date
  +gerarSelo()
  +validar()
}

class CertificadoOrigem {
  +id: int
  +numero: string
  +dataEmissao: date
  +emissor: string
  +gerar()
  +assinarDigitalmente()
}

class Expedicao {
  +id: int
  +dataArmazenamentoCofre: date
  +dataSaida: date
  +responsavel: string
  +destino: string
  +registrarEntradaCofre()
  +registrarSaida()
}

class Subproduto {
  +id: int
  +tipo: string
  +quantidade: float
  +dataRegistro: date
  +registrar()
}

class Equipamento {
  +id: int
  +tipo: string
  +modelo: string
  +fabricante: string
  +numeroSerie: string
  +alocarParaArea()
  +manutencaoPreventiva()
}

class Veiculo {
  +id: int
  +placa: string
  +modelo: string
  +fabricante: string
  +registrarMovimentacao()
}

class Funcionario {
  +id: int
  +nome: string
  +cpf: string
  +funcao: string
  +autenticar()
  +assumirResponsabilidade()
}

class Engenheiro {
  +cref: string
  +aprovarAtividade()
  +assinarRelatorio()
}

class Documento {
  +id: int
  +tipo: string
  +nomeArquivo: string
  +caminho: string
  +dataUpload: date
  +visualizar()
  +baixar()
}

class Mapa {
  +id: int
  +tipo: string
  +nomeArquivo: string
  +caminho: string
  +visualizar()
  +sobreporAreas()
}

class EstacaoMeteorologica {
  +id: int
  +codigo: string
  +localizacao: string
  +possuiPluviometro: bool
  +coletarDado()
  +exportar()
}

class DadoClimatico {
  +id: int
  +timestamp: datetime
  +precipitacao_mm: float
  +temperatura_C: float
  +umidade_relativa: float
  +velocidadeVento_ms: float
}

class Animal {
  +id: int
  +especie: string
  +statusConservacao: string
  +observacoes: string
  +registrarAvistamento()
}

class Arvore {
  +id: int
  +especie: string
  +diametro_cm: float
  +altura_m: float
  +registrarInventario()
}

class Camera {
  +id: int
  +fabricante: string
  +modelo: string
  +posicao: string
  +ativar()
  +desativar()
}

class Midia {
  +id: int
  +tipo: string
  +caminho: string
  +dataHora: datetime
  +visualizar()
  +exportar()
}

Empresa "1" *-- "1..*" Area
Empresa "1" *-- "0..*" Documento
Empresa "1" *-- "0..*" Mapa
Empresa "1" *-- "0..*" Funcionario
Empresa "1" *-- "0..*" Veiculo
Empresa "1" *-- "0..*" Equipamento
Empresa "1" *-- "0..*" LicencaExploracao
Empresa "1" *-- "0..1" EstacaoMeteorologica
Empresa "1" *-- "0..*" Animal
Empresa "1" *-- "0..*" Arvore
Empresa "1" *-- "0..*" Camera

Jazida --|> Area
ReservaLegal --|> Area
Patio --|> Area
Administrativa --|> Area

Area "1" *-- "3..*" Coordenada

Jazida "*" -- "*" Mineral

Area "1" *-- "0..*" AtividadeLavra
Area "1" *-- "0..*" LoteProducao
AtividadeLavra "1" --> "0..*" LoteProducao
AtividadeLavra "*" --> "1" Funcionario
LoteProducao "*" --> "1" Mineral
LoteProducao "1" o-- "0..*" TesteQualidade
TesteQualidade "0..*" --> "1" NivelPureza
LoteProducao "0..1" -- "1" SeloPureza
LoteProducao "0..1" o-- "1" Expedicao
LoteProducao "0..*" --> "0..*" Subproduto
LoteProducao "*" --> "0..1" CertificadoOrigem

Documento "0..*" --> "0..1" Area
Mapa "*" -- "*" Area

Equipamento "0..*" -- "*" Mineral
Equipamento "0..*" --> "0..1" Area
Veiculo "0..*" --> "0..1" Area
AtividadeLavra "0..*" --> "0..*" Equipamento
AtividadeLavra "0..*" --> "0..*" Veiculo

Engenheiro --|> Funcionario
Engenheiro "1" --> "0..*" Area
TesteQualidade "*" --> "1" Funcionario
Expedicao "*" --> "1" Funcionario

EstacaoMeteorologica "1" *-- "0..*" DadoClimatico
DadoClimatico "0..*" -- "0..*" Area

Area "0..*" --> "0..*" Camera
Camera "1" *-- "0..*" Midia
