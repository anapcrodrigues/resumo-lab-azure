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

### Tipos de serviço de nuvem: IaaS, PaaS e SaaS

**IaaS (infraestrutura como serviço)**
Tendem a ser estruturas/recursos que o usuário tem mais acesso no contexto de personalização daquele recurso, tem mais liberdade para configurar.

Exemplo: Crie uma infraestrutura de TI de pagamento conforme o uso alugando servidores, máquinas virtuais, armazenamento, redes e sistemas operacionais de um provedor de nuvem.

![IaaS](https://github.com/user-attachments/assets/195cfd7a-926e-4506-8df9-fb12ceaa2093)


**PaaS (plataforma como serviço)**
Fornece um ambiente para a criação, o teste e a implantação de aplicativos de software, sem focar no gerenciamento da infraestrutura subjacente.

![PaaS](https://github.com/user-attachments/assets/8a008490-8394-435b-90e3-4640298eeb56)


**SaaS (software como serviço)**
A aplicação já existe, já se conhece o que a aplicação entrega e o que determina o meu acesso a aplicação é a opção de licenciamento escolhida.
Os usuários se conectam e usam aplicativos com base em nuvem pela internet. Exemplo: Microsoft Office 365, email e calendários.

![SaaS](https://github.com/user-attachments/assets/612abcf0-e396-4efc-956b-dae9bfd1faf0)

**Modelo de responsabilidade compartilhada**

![Modelo de responsabilidade compartilhada](https://github.com/user-attachments/assets/415c5c0d-f633-4595-9518-f4efef769817)

#### Comparação do serviço de nuvem

**IaaS**
- O serviço de nuvem mais flexível.
- Você configura e gerencia o hardware para seu aplicativo.

**PaaS**
- Focado no desenvolvimento de aplicativos.
- O gerenciamento de plataforma é realizado pelo provedor de nuvem.

**SaaS**
- Modelo de preço de pagamento conforme o uso.
- Os usuários pagam pelo software que utilizam em um modelo de assinatura (licenciamento).


## Componentes de Arquitetura do Azure
### Regiões
É possível criar recursos em vários lugares do mundo.
- As regiões são compostas de um ou mais datacenters muito próximos.
- Elas fornecem flexibilidade e escala para reduzir a latência do cliente.
- As regiões preservam a residência dos dados com uma oferta abrangente de conformidade.

### Zonas de disponibilidade
- Fornece proteção contra tempo de inatividade devido a falha do datacenter.
- Separa fisicamente os datacenters dentro da mesma região.
- Cada datacenter é equipado com alimentação, resfriamento e rede independentes.
- Os datacenters são conectados por meio de redes privadas de fibra óptica para reduzir latência.
