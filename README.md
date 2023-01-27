# C# com .Net

### Requisitos não funcionais

````
⦁	Seu desafio deverá ser feito em .Net.
⦁	A versão pode ser escolhida pelo executor.
⦁	A parte de front-end deverá estar em ASP.Net MVC.
⦁	Deverá haver emprego de testes unitários (Somente para Sênior).
⦁	Deverá haver emprego de DDD (Somente para Sênior).
⦁	Deverá haver emprego de Paralelismo (Para Pleno e Sênior).
⦁	Os métodos deverão ser assíncronos.
⦁	Componentes plugáveis (Somente para Sênior).
⦁	Documentação de requisitos e escopo de execução (Somente para Sênior).
 ````

## Requisitos funcionais

#### Introdução

----
Chicorita Folhagem é uma analista de Recursos Humanos e mensalmente ela recebe uma série de arquivos dos diferentes departamentos para executar o fechamento do ponto e emitir a ordem de pagamento.
Para emitir a ordem de pagamento Chicorita precisa validar os dias trabalhados e também as horas trabalhadas em cada dia.
----

## Nos arquivos recebidos, Chicorita ao observar cada Pessoa valida os seguintes requisitos:
 ````
⦁	Dias trabalhados. O trabalho segue de segunda a sexta e é esperado que o funcionário trabalhe 8 horas por dia mais 1 hora de almoço.
⦁	Valor da hora da pessoa.
⦁	Os dias não trabalhados são descontados da pessoa.
⦁	Horas não trabalhadas são descontadas da pessoa.
⦁	Horas extras são pagas.
⦁	Dias extras são pagos.
 ````
 
## Após a análise de Chicorita é gerado um arquivo contendo as seguintes informações:
 ````
⦁	O valor pago por departamento.
⦁	Os dados da pessoa.
⦁	Valor pago a cada pessoa.
⦁	Valor descontado de cada pessoa.
⦁	Quantidade de horas extras ou horas faltantes. Quando as horas são faltantes Chicorita coloca o valor negativo.
⦁	Quantidade de dias extras ou faltantes. Quando os dias são faltantes Chicorita coloca o valor negativo.
 ````
 
# Requisitos do sistema

### O sistema pode ser um MVC ou um Console Application, mas ele deverá:

````
⦁	Ser feito em .Net (Qualquer versão).
⦁	Deverá conter um arquivo Readme com as informações do projeto.
⦁	Ler todos os arquivos da pasta designada. Exemplo: “C:\Arquivo a Importar\”.
⦁	A pasta deverá ser informada na hora em input feito pelo usuário.
⦁	Processar os arquivos em paralelo para aumentar o desempenho (Júniors não precisa fazer em paralelo). Chicorita recebe em torno de 1000 arquivos com aproximadamente 10000 informações de usuário. (Sim, ela não dá conta de fazer tudo e por isso temos muito erro no RH - )
⦁	Se tiver uma solução melhor para resolver o problema de desempenho pode usar.
⦁	Os arquivos recebidos estão no formato CSV, Chicorita tenta fazer o cálculo de tudo importando os arquivos no Excel e usando formulas que ela já conhece.
⦁	Nome do arquivo contém: Nome do Departamento, Mês de vigência, Ano de vigência. Exemplo: ‘Departamento de Operações Especiais-Abril-2022.csv’
⦁	O arquivo contém as seguintes colunas: Código: número, Nome: Texto, Valor hora: Dinheiro, Data: Dia do registro, Entrada: Hora do registro, Saída: Hora do registro, Almoço: Hora de registro
 ````

Essa imagem é ilustrativa, na realidade os dados não irão chegar de forma ordenada, mas serão formatados como neste exemplo. 
Haverá mais funcionários e não há qualquer ordenação referente à data, código, nome ou qualquer outro campo.
Observe que as colunas serão separadas por ponto e vírgula.

````Código;Nome;Valor hora;Data;Entrada;Saída;Almoço````

````
⦁	O sistema deverá gerar uma saída no formato JSon. Um único arquivo para todos os departamentos. Será formatado como na imagem abaixo:
 ````


### Para finalizar, pedimos que você crie um Projeto com ASP.Net MVC com uma Duas Views estáticas.

 ````
⦁	Home: Contendo o nome do candidato; Cargo pretendido; Pretensão salarial; Data do teste.
⦁	About: Gostaria que você colocasse um texto informando qual desafio de programação mais marcou sua jornada até o momento.
 ````
 
### Neste texto queria que você colocasse: Tecnologia usada, Arquitetura, Como você atuou e por que te marcou tanto este desafio.
