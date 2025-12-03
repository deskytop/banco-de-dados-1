# 🗺️ [Lista de Exercício 1](./../assets/files/Lista%20de%20Exercicios%201.pdf) - Guia
[Voltar ao Início](./../README.md)
***
## 💻 Questões Práticas 
| Questão  | Resolução |
| --- | :---: |
| Prática 1 - Livraria | [ 🟢 ](./questao-6) |
| Prática 2 - Hospital | [ 🟢 ](./questao-7) |
| Prática 3 - Escola | [ 🟢 ](./questao-9) |
| Prática 4 - Projeto Livre | [ 🟢 ](./questao-10) |

## 📄 Questões teóricas
    1. Explique a importância da modelagem conceitual no processo de desenvolvimento de
	sistemas de informação. Relacione sua resposta com a independência de dados e a
	comunicação entre usuários e desenvolvedores.

_R= A modelagem conceitual é fundamental no desenvolvimento de sistemas porque cria um diagrama de alto nível (como o Entidade-Relacionamento) que funciona como uma linguagem universal. Isso permite que usuários e gestores validem se suas regras de negócio foram compreendidas corretamente pelos desenvolvedores, antes do início da programação. Ao mesmo tempo, essa abordagem estabelece a independência de dados, pois define a estrutura da informação com base no negócio, e não na tecnologia, permitindo que o sistema evolua ou mude de plataforma com impacto mínimo nas aplicações._

    2. Diferencie entidade forte de entidade fraca. Forneça um exemplo prático de cada uma
	em um sistema de gestão acadêmica.

_R= Uma entidade forte existe por si só e tem uma chave primária própria (ex: CURSO, identificado por codigo_curso). Uma entidade fraca depende de uma entidade forte para existir e só é identificada unicamente pela chave da entidade forte mais um atributo seu (ex: DISCIPLINA, identificada por codigo_curso + codigo_disciplina)._

    3. Defina e compare os conceitos de chave primária, chave candidata e superchave.
	Explique por que a escolha correta da chave primária é fundamental.

_R= 
Superchave: Qualquer conjunto de atributos que identifica unicamente uma linha (ex: {cpf, nome})._

_Chave Candidata: É uma superchave mínima, sem atributos redundantes (ex: {cpf})._

_Chave Primária: É a chave candidata escolhida para ser o identificador principal da tabela._

_A escolha correta da chave primária é fundamental porque ela garante a unicidade dos dados, é a base para criar relacionamentos entre tabelas e otimiza a performance das consultas._

    4. O que são relacionamentos ternários em um modelo entidade-relacionamento (MER)?
	Dê um exemplo de situação em que esse tipo de relacionamento é necessário.

_R= Um relacionamento ternário é a associação simultânea de três entidades distintas para registrar um fato único que perderia o sentido se fosse dividido, como um MÉDICO que prescreve um MEDICAMENTO para um PACIENTE._

    5. Descreva o papel dos atributos multivalorados e derivados em um MER. Explique como
	representá-los e quando é recomendável normalizar sua representação.


_R= Atributo Multivalorado: Permite vários valores para uma entidade (ex: telefones de um cliente). É representado por uma elipse dupla e, ao criar o banco de dados, deve ser normalizado, tornando-se uma nova tabela separada._

_Atributo Derivado: Seu valor é calculado a partir de outros atributos (ex: idade a partir da data_nascimento). É representado por uma elipse tracejada e, geralmente, não é armazenado na tabela, sendo calculado pela aplicação quando necessário para garantir consistência._
***
[Voltar ao Início](./../README.md)