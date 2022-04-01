# ENTENDENDO COMO O GIT FUNCIONA    
#### O que é SHA? ####
É uma codificação de programas por encriptação, gerando um conjunto de caracteres identificador único, sendo ele usado para identificar os arquivos.      
#### TIPOS DE OBJETOS RESPONSAVEIS PELO VERSIONAMENTO DO CÓDIGO -OBJETOS FUNDAMENTAIS ####

*bloco básico de composição.*   
☁️ **BLOBS (bolhas)**: informações de tipo, tamanho do arquivo, \0 e conteúdo do arquivo (METADADOS)

*armazena e aponta para diferentes BLOBS, responsaveis por montar a estrutura de localização dos arquivos.*     
🌳**TREES**: informações de armazenamento das BLOBS, SHA
e nome do arquivo

*junção de todas as informações do arquivo.*    
💾**COMMITS**: objeto que junta todos os itens, aponta a TREE, parente, autor, mensagem e timestamp (carimbo de tempo), tem SHA1 criptação dos seus metadados e se vc altera 
o dado dentro de uma BLOB gera um SHA1, e altera os metadados da TREE e o COMMIT.

#### O commit garante a verificação de dados e alterações no arquivo, é uma forma segura de acertificar que ninguem mexeu no código. ####

#### COMANDOS DO GIT ####

**GIT INIT:** iniciar repositorio     
**GIT ADD:** mover arquivos     
**GIT COMMIT:** criar commit  
**GIT STATUS:** mostra o status dos arquivos modificados e não modificados  
**GIT CLONE:** faz uma cópia do link usado para rede particular       
**GIT ADD . (-A):** adiciona alterações no arquivo modificado       
**GIT PUSH ORIGIN MAIN:** envia versão finalizada
