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




### PLANILHA COM TODOS OS TESTES FEITOS: 
[Testes](https://docs.google.com/spreadsheets/d/1s_RWD_LDLQcjtSbKFMWoC29V2wF_irup5TOS6ehNhac/edit?usp=sharing)





 # TESTE DE FLUXO : 
[Fluxo cadastro com sucesso](https://drive.google.com/file/d/1320PlBktSbW9gi9s6HKq2eTyHXJsBWc4/view?usp=sharing)



# LISTAGEM : 
[Lista de cursos ](https://drive.google.com/file/d/1-Ga892SKvWPa5IoEnHZDDsy_LS3tfyQr/view?usp=sharing)


# CENÁRIOS NEGATIVOS: 
Resultados inesperados: 

# FALHA NA VALIDAÇÃO DE REQUIREMENT FIELDS
Campos podem ser ignorados e pode-se entregar o curso sem preenchimento de dados impossibilitando a validação 

# INPUT DE DADOS; 
Os inputs de nome/ número apresentam problemas como : Em vez de colocar letras no espaço de nome pode- se colocar números e será aceito 
O link da imagem não precisa ser preenchido com um link de imagem válido 
Campos como instrutor aceitam números, descrição também aceitam números ao invés de palavras que seria o resultado esperado 
Endereço pode aceitar palavras que não sejam endereços físicos mas sim palavras soltas 





# VÍDEO COM TODOS OS CENÁRIOS NEGATIVOS : 
[Cenários Negativos e Validações](https://drive.google.com/file/d/17xQvivVEYRywlfjbWq2vy_XtpUUvcd7s/view?usp=sharing) 




# PROBLEMA DE INTERFACE : 
1ª Página inicial 

2 ª Na aba de listar cursos

3 ª Se você rolar a página para baixo e estiver com muitos cursos a página ficará dessa forma: 


[Problema de Interface - Listagem de Cursos](https://drive.google.com/file/d/1-JuF3HNLogQ3iRyOFnuHu7TI8XTapcPg/view?usp=sharing)


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



#  Observação :  deixei os bugs somente no github pois acredito que seja melhor por conta das descrições pedidas conforme o formulário. Mas todos os testes negativos se encontram no vídeo abaixo. 
Deixei o problema de interface também porque queria dar uma sugestão de melhoria. 

Melhoria que poderia ter na plataforma: acessibilidade para pessoas surdas e/ou mudas 

Obrigado pela oportunidade 









