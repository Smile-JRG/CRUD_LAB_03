# Cadastro_Clinica_Medica

<h1 align="center"> Clinica médica - Cadastro de médicos e pacientes </h1>


<!-- INTRODUÇÃO -->
## 📝 DESCRIÇÃO DO PROJETO:
<p align="center">O objetivo desse Projeto é utilizar o Spring Boot para desenvolver uma API Rest, com algumas funcionalidades. A ideia é desenvolver um CRUD, sendo as quatro operações fundamentais das aplicações: cadastro, leitura, atualização e exclusão de informações.

Isto é, será desenvolvido um CRUD de uma API Rest usando o Spring Boot.
Trabalharemos em um projeto de uma clínica médica fictícia, que precisa de um aplicativo para monitorar o cadastro de médicos, pacientes e agendamento de consultas.

Será um aplicativo com algumas opções, em que a pessoa que for usar pode fazer o CRUD, tanto de médicos quanto de pacientes e o agendamento e cancelamento das consultas.</p>

<!-- DESENVOLVEDORES -->
## 👨🏻‍💻 DESENVOLVEDORES

<p align="center"> 
 Meu nome é <b>Jose Ricardo Gustavo - RA: 202114786</b>, sou bastante interessado por tecnologia e trabalho a aproximadamente vinte anos na área de manutenção industrial, sendo que, nos últimos dez anos tenho atuado especificamente com assistência técnica de máquinas injetoras plástica e robôs cartesianos. Iniciei meu estudo profissionalizante em 2002 no SENAI e conclui minha primeira graduação em 2009, no curso de Tecnólogo em Automação Industrial - UniAnchieta. Ingressei no curso de Engenharia de Computação - USF com o intuito de adquirir um conhecimento mais especializado.
</p>


<!-- FERRAMENTAS UTILIZADAS -->
## 🧰 DESENVOLVIDO COM AS SEGUINTES FERRAMENTAS:

<table>
  <tr>
    <td><bold>Application</bold></td>
    <td><bold>Version</bold></td>
  </tr>
  <tr>
    <td>Spring Boot 3</td>
  </tr>
   <tr>
    <td>Java 17</td>
  </tr>
    </tr>
   <tr>
    <td>Lombok</td>
  </tr>
 <tr>
    <td>MySQL/Flyway</td>
  </tr>
   <tr>
    <td>JPA</td>
  </tr>
    </tr>
   <tr>
    <td>Maven</td>
   </tr>
   <tr>
    <td>Insomnia</td


</table>

<!-- FUNCIONALIDADES -->
## ⚙️ FUNCIONALIDADES

<h3>1. Cadastro de Pacotes (Create):</h3>
<ul>Permite a adição de novos pacotes de viagens. Sendo possível inserir o local de destino, data de saída,volta e o preço das acomodações.</ul>

<h3>2. Consulta de Pacotes (Read):</h3>
<ul>Fornece uma vizualização de todos pacotes disponíveis, contendo seu preço e as datas disponíveis.</ul>

<h3>3. Atualizações (Update):</h3>
<ul>Possibilita a edição de detalhes dos pacotes de viagens, a fim de corrigir preços, datas e locais.</ul>

<h3>4. Remoção de Pacotes (Delete):</h3>
<ul>Permite a exclusão de pacotes não disponíveis. Garatindo que cada viagem seja existente e possível.</ul>

<p align="center">
Tudo isso foi feito usando algumas tecnologias, como Spring Boot 3, sendo a última versão disponibilizada pelo framework. 

Será utilizado em conjunto com o projeto o Lombok, responsável por fazer a geração de códigos repetitivos, como getters, setters, toString, entre outros. Tudo via anotações para o código ficar menos escrito.

Também será utilizado o banco de dados MySQL para armazenar as informações da API e junto com ele utilizaremos a biblioteca Flyway. Isso para termos o controle do histórico de evolução do banco de dados, um conceito que chamamos de Migration.

A camada de persistência da aplicação será feita com a JPA (Java Persistence API), com o Hibernate como implementação dessa especificação e usando os módulos do Spring Boot, para tornar esse processo o mais simples possível.

Usaremos o Maven para gerenciar as dependências do projeto, e também para gerar o build da nossa aplicação. Por último, como focaremos na API Rest (apenas no Back-end), não teremos interface gráfica, como páginas HTML e nem Front-end e aplicativo mobile.

Mas para testarmos a API, usaremos o Insomnia, sendo uma ferramenta usada para testes em API. Com ela, conseguimos simular a requisição para a API e verificar se as funcionalidades implementadas estão funcionando.
</p>

<br>

<!-- REPOSITÓRIO -->
<h2 align="left">📁 PROJETO: </h2>

- Clonar o Repositório <br>
  `git clone https://github.com/EullerFPassos/github

- Arquivos Git no logo abaixo: <br>
<a href="https://github.com/EullerFPassos/github.git">
  <img src="https://cdn.icon-icons.com/icons2/1673/PNG/512/downloadoutline_110860.png" alt="GitHub" style="width:50px;">
</a>

<br>

<!-- POSTMAN -->
## ✔️ EXEMPLO DE FUNCIONAMENTO:

<h4>agenicaController:</h4>

   - `GET`
      - Endpoint: `/pacotes`
      - Exemplo de Saída:
      ```bash
      [
         {

	public record DadosCadastroPaciente(

        String nome,
        String email,
        String telefone,
        String cpf,
        DadosEndereco endereco
	) 

	 }
      ]
      ```

   - `POST`
     - Endpoint: `/pacotes`
     - Exemplo de entrada:
     ```bash
     [
         {
        "nome":"Rodrigo Ferreira",
	"email":"rodrigo.ferreira@voll.med",
	"crm":"123456",
	"especialidade":"ortopedia",
	"endereco":{
    	"logradouro":"rua 1",
    	"bairro":"bairro",
    	"cep:"12345678",
    	"cidade":"Brasilia,
    	"uf":"DF",
    	"numero":"1",
    	"complemento":"complemento",
   	 	   }
         }
     ]
     ```
  
  - `PUT`
      - Endpoint: `/pacotes/{id}`
      - Exemplo de entrada:
      ```bash
      [
          public void atualizarInformacoes(DadosEndereco dados) {

        if (dados.logradouro() != null) {
            this.logradouro = dados.logradouro();
        }
        if (dados.bairro() != null) {
            this.bairro = dados.bairro();
        }
        if (dados.cep() != null) {
            this.cep = dados.cep();
        }
        if (dados.uf() != null) {
            this.uf = dados.uf();
        }
        if (dados.cidade() != null) {
            this.cidade = dados.cidade();
        }
        if (dados.numero() != null) {
            this.numero = dados.numero();
        }
        if (dados.complemento() != null) {
            this.complemento = dados.complemento();
        }
    }
}
      ]
      ```

  - `DELETE`
      - Endpoint: `/pacotes/{id}`
      - Exemplo de entrada:
      ```bash
      [
        @DeleteMapping("/{id}")
    	@Transactional
    	public void excluir(@PathVariable Long id) {
        var medico = repository.getReferenceById(id);
        medico.excluir();
    }

    public void excluir() {
        this.ativo = false;
    }


     ]
       ```
 
