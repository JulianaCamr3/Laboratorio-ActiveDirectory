# Laboratório Active Directory

## Objetivo
Este laboratório tem como objetivo demonstrar o uso do **Active Directory** na administração de ambientes corporativos.As atividades incluem:  

- Gerenciamento de usuários e computadores.
- Aplicação de **Group Policies** para diferentes perfis.
- Configuração de métodos de autenticação.

## Competências desenvolvidas

- Administração de sistemas Windows Server
- Implementação de políticas de segurança
- Organização e controle de infraestrutura de TI

## Administração de Usuários

O primeiro laboratório consistiu na exclusão de todos os usuários de um departamento que não permanecem na empresa. A remoção adequada de contas é fundamental para garantir a segurança da organização, pois acessos indevidos podem resultar em vazamento de dados, prejuízos financeiros e violação do princípio da confidencialidade da informação.

**Nas imagens a seguir, eu mostro o passo a passo para excluir corretamente esse departamento no Active Directory.**

Na primeira imagem, é possível analisar a tela que possui a pasta  THM que contém todos os departamentos da empresa. O departamento que queremos excluir é o "Research and Development". Por padrão, o AD possui um mecanismo para evitar a exclusão de alguma pasta por acidente, então se apenas formos até a pasta do departamento para excluir, receberemos uma mensagem de erro. Para desativar esse mecanismo de proteção precisamos ir até o canto superior, na aba *View*

Então, para desativar esse mecanismo de proteção precisamos ir até o canto superior, na aba *View* e selecionar a opção *Advanced Features*.

![Active Directory Users and Computers](imagens/LaboratorioActiveDirectory1.png)


![Clicando em Advanced Features](imagens/LaboratorioActiveDirectory2.png)

Em seguida, acessamos a pasta *Research and Development*, clicamos com o botão direito e selecionamos a opção *Properties*. A partir dessa seção, clicamos na opção *Object* no canto supeior e desmarcamos a opção **Protect object from accidental deletion**. Após realizarmos essas operações, será possível excluir a pasta adequadamente

![Clicando em Properties](imagens/LaboratorioActiveDirectory3.png)
![Desmarcando o mecanismo de proteção](imagens/LaboratorioActiveDirectory4.png)
![Opção desmarcada](imagens/LaboratorioActiveDirectory5.png)
