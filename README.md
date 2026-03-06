# DESAFIO-QA-BEEDOO-2026
Repositório de testes manuais que fiz para um desafio de qa para a empresa beedoo para uma entrevista técnica. 

# Qual você acredita ser o objetivo da aplicação?
O objetivo da aplicação me parece ser uma  listagem de cursos   para  uma instituição de cursos técnicos ou profissionalizantes, mas parece ser um grupo grande devido a quantidade de cursos que podemos cadastrar. 

# Quais são os principais fluxos disponíveis  ? 
Ao entrarmos na aplicação temos duas opções disponíveis mas  a listar cursos primeira opção depende do fluxo do cadastro 
Os fluxos são o cadastro completo com todos os dados sendo preenchidos
para isso vá em cadastrar curso > preencha todos os campos corretamente e clique em cadastrar e ele será cadastrado, uma vez cadastrado poderá clicar em listar cursos e ele aparecerá normalmente. 

# Quais pontos do sistema você considera mais críticos para teste ? 
 Os pontos mais  críticos para mim foram os campos de seção que não são obrigatórios e te permitem cadastrar o curso sem nenhum dado, também o de datas antigas que te permite colocar uma data de término anterior a do início e o contrário também é verdade te permite fazer uma data de início posterior a data de término. 

 
#  TESTE DE FLUXO : 
Para realizar esse teste, 
1 ª basta acessar > 2ª  cadastrar curso > 3ª  preencher todos os campos obrigatórios > 4ª  selecionando corretamente todas as opções e o seu curso será cadastrado na listagem de cursos  

# RESULTADO ESPERADO: O CURSO APARECERÁ NA LISTAGEM (ALCANÇADO) 
[Fluxo cadastro com sucesso](https://drive.google.com/file/d/1320PlBktSbW9gi9s6HKq2eTyHXJsBWc4/view?usp=sharing)



# LISTAGEM:
Para acessar é só clicar Listar cursos: já adianto a interface acho que está bugada provavelmente com containers maiores do que deveriam e não totalmente espaçados de um jeito esperado. 
[Lista de cursos ](https://drive.google.com/file/d/1-Ga892SKvWPa5IoEnHZDDsy_LS3tfyQr/view?usp=sharing)


# CENÁRIOS NEGATIVOS: 
Resultados inesperados: 

# FALHA NA VALIDAÇÃO DE REQUIREMENT FIELDS
Campos podem ser ignorados e pode-se entregar o curso sem preenchimento de dados impossibilitando a validação 

# PASSO A PASSO ;
 1ª  Clique em cadastrar curso  

 2ª Não preencha nenhum campo 
 
 3ª Clique em Cadastrar Curso 

 # RESULTADO ESPERADO: A APLICAÇÃO PEDIR PARA O USUÁRIO PREENCHER OS CAMPOS OBRIGATÓRIOS (NÃO ALCANÇADO) 

# INPUT DE DADOS; 
Os inputs de nome/ número apresentam problemas como : Em vez de colocar letras no espaço de nome pode- se colocar números e será aceito 
O link da imagem não precisa ser preenchido com um link de imagem válido 
Campos como instrutor aceitam números, descrição também aceitam números ao invés de palavras que seria o resultado esperado 
Endereço pode aceitar palavras que não sejam endereços físicos mas sim palavras soltas 

# PASSO A PASSO INVALIDAÇÃO DE CAMPOS : 
1ª Página inicial 

2 ª Clique em cadastrar curso 

3 ª No campo de nome preencha com números 

4 ª Clique  em cadastrar curso 

# RESULTADO ESPERADO: O CAMPO  NOME SÓ ACEITAR LETRAS (NÃO ALCANÇADO)

# PASSO A PASSO INVALIDAÇÃO DE CAMPOS : 
1ª Página inicial 

2 ª Clique em cadastrar curso 

3 ª No campo de instrutor  preencha com números 

4 ª Clique  em cadastrar curso 

# RESULTADO ESPERADO: O CAMPO  INSTRUTOR  SÓ ACEITAR LETRAS (NÃO ALCANÇADO)

# PASSO A PASSO INVALIDAÇÃO DE CAMPOS : 
1ª Página inicial 

2 ª Clique em cadastrar curso 

3 ª No campo de descrição   preencha com números 

4 ª Clique  em cadastrar curso 

# RESULTADO ESPERADO: O CAMPO  DESCRIÇÃO   SÓ ACEITAR LETRAS (NÃO ALCANÇADO)

# PASSO A PASSO INVALIDAÇÃO DE CAMPOS : 
1ª Página inicial 

2 ª Clique em cadastrar curso 

3 ª No campo de endereço   preencha  somente com números 

4 ª Clique  em cadastrar curso 

# RESULTADO ESPERADO: O CAMPO ENDEREÇO    ACEITAR VALORES VÁLIDOS  (NÃO ALCANÇADO)

# VALIDAÇÃO DE IMAGEM 
1 ª Página inicial da aplicação 

2 ª Cadastrar curso 

3 ª Clicar em url da imagem 

4 ª Copiar qualquer url  de qualquer aplicação

5 ª Colar a url  que não é uma imagem 

6 ª Clicar em cadastrar curso 

# RESULTADO ESPERADO QUE SOMENTE LINKS DE IMAGEM SEJAM VÁLIDOS PARA O CAMPO (RESULTADO NÃO ALCANÇADO) 

# PROBLEMA DE INTERFACE : 
1ª Página inicial 

2 ª Na aba de listar cursos

3 ª Se você rolar a página para baixo e estiver com muitos cursos a página ficará dessa forma: 



 # RESULTADO ESPERADO DA INTERFACE PARA MELHOR EXPERIÊNCIA  QUE OS CURSOS FICASSEM LADO A LADO : 
 <img width="1815" height="442" alt="image" src="https://github.com/user-attachments/assets/dccbf86a-7b40-4ff3-bcc3-123de3ddcee1" />

 # EXEMPLO DE INTERFACE COM OS CONTAINERS LADO A LADO DA PLATAFORMA UDEMY 



# BUG DE EXCLUSÃO 

ª1 Página inicial 

2ª Cadastre qualquer curso 

3ª Volte para a página de listagem de cursos

4ª Tente excluir o curso 

# RESULTADO ATUAL: O CURSO NÃO IRÁ SER EXCLUIDO, ELE PERMANECERÁ NA LISTAGEM 

# RESULTADO ESPERADO: QUE O CURSO NÃO APARECESSE MAIS NA ABA DE LISTAGEM DE CURSOS 

Erro de funcionalidade, impacto: bloqueio de fluxo pois se precisar excluir algum curso para cadastrar outro não terá como impedindo o fluxo de atualização da aplicação 


# BUG DE VISUALIZAÇÃO 

ª1 Página inicial 

2ª Cadastre qualquer curso 

3ª Volte para a página de listagem de cursos

4ª Tente visualizar o curso   

# RESULTADO ATUAL: O CURSO NÃO IRÁ SER VISUALIZADO, OS DADOS DELE ESTARÃO BLOQUEADOS PARA A CONSULTA

# RESULTADO ESPERADO: QUE OS DADOS DO CURSO APARECESSEM QUANDO VOCÊ CLICASSE

 Erro de funcionalidade, impacto: bloqueio de fluxo pois se precisar atualizar  alguma informação  cadastral  o aluno  não terá como assim  impedindo o fluxo de atualização dos dados cadastrais do aluno. 

# VÍDEOS COM TODOS OS CENÁRIOS NEGATIVOS : 
[Cenários Negativos e Validações](https://drive.google.com/file/d/17xQvivVEYRywlfjbWq2vy_XtpUUvcd7s/view?usp=sharing)






# TESTES DE TODOS ESSES CENARIOS
: https://drive.google.com/file/d/17xQvivVEYRywlfjbWq2vy_XtpUUvcd7s/view?usp=sharing 



