# Resumo lab Microsoft Azure Essentials

## Objetivo
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab Microsoft Azure Essentials na DIO.

## Sumário



## Conceitos de nuvem
### Benefícios da nuvem

**Alta disponibilidade**
A alta disponibilidade se concentra em garantir a disponibilidade máxima, independentemente de interrupções ou eventos que possam ocorrer.
Altamente relacionado ao SLA da Microsoft que garante que o serviço estará disponível (up time) de acordo com o concordado em contrato. Quando maior o up time, mais caro será. Caso o SLA de up time não seja atendido, a Microsoft dará um crédito à empresa.

**Escalabilidade**
Refere-se à capacidade de ajustar recursos para atender à demanda. A capacidade de escalar significa que você poderá adicionar mais recursos para lidar melhor com o aumento da demanda.
Um benefício da escalabilidade é que você não está pagando além do necessário pelos serviços, pois em nuvem você paga apenas pelo que usa.
Com a escala vertical é possível adicionar mais CPUs ou RAM à máquina virtual, caso precisasse de mais capacidade de processamento.

**Elasticidade**
Diferente da escalabilidade, em que eu sei o quanto é a minha demanda, elasticidade atende em situações em que minha demanda é desconhecida. Por exemplo, se houvesse um salto repentino acentuado na demanda, os recursos implantados poderiam ser expandidos (automaticamente ou manualmente). O mesmo é válido para reduzir recursos. Um bom exemplo de situação como essa é a black friday.

**Confiabilidade**
Devido ao design descentralizado, a nuvem naturalmente dá suporte a uma infraestrutura confiável e resiliente. Também permite implantar recursos em várias regiões do mundo. 
Assim, é possível criar ambientes de disaster recovery, mesmo que ocorra eventos catastróficos em uma região, as outras regiões ainda estarão funcionando.

**Previsibilidade**
A previsibilidade na nuvem permite que você avance com confiança, seja no desempenho ou no custo. Ambas são influenciadas pelo Microsoft Azure Well-Architected Framework.

**Segurança**
A nuvem oferece ferramentas de segurança, mas é importante lembrar que a implementação de muitas delas devem ser realizadas pelo cliente. A implementação de ferramentas de segurança NÃO É FEITA PELA MICROSOFT, é de responsabilidade do cliente.
O provider é responsável por oferecer recursos e serviços para atender a demanda de segurança, o cliente é o responsável por aplicá-las.

**Governança**
A auditoria baseada em nuvem ajuda a sinalizar qualquer recurso que esteja fora de conformidade com os padrões corporativos e fornece estratégias de mitigação.
Aplica padrões e regras de maneira mais facilitada.
Ao estabelecer uma presença de governança o mais cedo possível, você poderá manter sua presença de nuvem atualizada, protegida e bem gerenciada.

**Gerenciabilidade**
O benefício é facilitar o gerenciamento através de opções de capacidade de gerenciamento.
Há dois tipos de capacidade de gerenciamento para computação em nuvem. O gerenciamento na nuvem diz respeito à maneira de gerenciar seu ambiente de nuvem e seus recursos. Por exemplo:
- Por meio de um portal da Web.
- Usando uma interface de linha de comando: usando APIs, PowerShell.
