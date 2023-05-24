------ CRÉDITOS
AUTOR: https://github.com/nikarmin/cinema-crud


------ Exercício de Tópicos Especiais em Sistemas para Internet
Grupo: Felipe Quaresma, Helton Vinícius, Josemo Junior e Lucas Bazante

Pesquisar por um sistema organizado como arquitetura orientada a serviços:
• Descrever suas tecnologias;
• Descrever a sua estrutura;
• Descrever os seus serviços;


Análise:
	
	Programa em Java que implementa um sistema de CRUD (Create, Read, Update, Delete) para gerenciar informações de um cinema. O programa oferece um menu interativo que permite ao usuário realizar diversas operações, como adicionar, visualizar, atualizar e excluir registros relacionados ao cinema. Além disso, o programa utiliza um WebService para fazer uma chamada REST a fim de obter informações detalhadas do CEP fornecido pelo usuário, enriquecendo assim os dados cadastrados para cada cinema no sistema.
	
	O serviço começa puxando o CEP do objeto da classe Cinema na aplicação em Java. A aplicação faz uma chamada HTTP usando o método GET para a API REST (https://api.postmon.com.br/v1/cep/). O CEP é incluído na URL da chamada como um parâmetro. A API REST recebe a requisição GET com o CEP fornecido e processa a solicitação. Ela consulta a fonte de dados ou o sistema responsável por obter os dados do endereço associado ao CEP.

	Em seguida, a API REST retorna uma resposta ao cliente (a aplicação em Java) no formato JSON, retornando informações como o bairro e o logradouro. Além disso, o JSON também inclui informações sobre o estado e cidade como: nome, área em quilômetros quadrados e o código IBGE.
	
	A estrutura de pacotes indica um projeto simples, focado em uma única funcionalidade ou com escopo limitado. Está mais alinhado com o MVC que inclui chamada de microsserviços.
