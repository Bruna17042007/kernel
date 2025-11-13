Qual foi a versão do kernel que você compilou, e por que escolheu essa versão?
 Compilei a versão 6.6.54 por ser uma das mais recentes e estáveis disponíveis no site oficial do Linux Kernel, oferecendo melhorias e correções de segurança.

 Que configuração você modificou no menuconfig? Por que fez essa modificação? O que espera que essa modificação altere no comportamento do sistema?
 Desabilitei o suporte a um sistema de arquivos que não utilizo (ex: NFS). Fiz isso para reduzir o tamanho final do kernel e otimizar o tempo de compilação.

Durante a compilação você encontrou algum erro, advertência ou comportamento inesperado? Como resolveu ou o que faria para resolver?
Sim, inicialmente apareceu o erro sobre a versão do GNU Make ser antiga.
 Resolvi atualizando o pacote com:
sudo apt install make
Depois disso, a compilação seguiu normalmente.

Quais os riscos e benefícios de “rodar” um kernel compilado por você mesmo em comparação com usar o kernel padrão da distribuição?
Benefícios: Possibilidade de personalizar recursos, drivers e otimizações, kernel mais leve e adequado ao hardware. 
Riscos: Erros de configuração podem impedir o sistema de inicializar, falta de suporte oficial da distribuição.

Em quais cenários você considera “vale a pena” compilar seu próprio kernel? Cite ao menos dois.
Quando é necessário suporte a hardware específico que não existe no kernel padrão.
Em ambientes de pesquisa, otimização ou segurança, onde é preciso ter controle total sobre o sistema.

Se o sistema não inicializar após a compilação/instalação do kernel, qual seria seu plano de contingência para recuperar o sistema?
Inicializar usando o kernel anterior através das “Opções Avançadas” do GRUB, e depois corrigir a instalação ou configuração do kernel novo.
