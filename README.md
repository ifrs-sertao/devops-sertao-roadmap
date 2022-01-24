# devops-sertao-roadmap
Proposta para construirmos junto nossa jornada de automação, infra as code, nuvem e DevOps.

# A ideia
Desde que iniciamos, ainda que intuitivamente, com ideias de automatizar processos para reduzir trabalhos manuais, adotamos várias técnicas e ferramentas. Penso que ainda falta nos coordenarmos para desenvolver conhecimento em grupo e definir ferramentas e fluxos padrão do setor, ainda mais agora que temos capacidade de desenvolver código.

# Mapa de Ferramentas/Tecnologias já adotadas no contexto de automação e redução do trabalho árduo(toil)
Tabela de recursos que já usamos de forma relativamente consolidada. Nota-se que, mesmo estratégias tradicionais( controle de domínio) trouxeram valor em termos de reduzir nossas tarefas penosas, manuais, individualizadas, o que otimiza o nosso trabalho.
Recurso                      | Resultado |
-----------------------------| -----------
Controlador de Domínio       | Incluindo as GPOs e limitação das permissões aos usuários nos PCs, automatizamos o mampeamentos e reduziu bastante incidentes causados pelos usuários
Servidor de Impressão | Reduziu o trabalho manual de instalação de impressoras
FogServer|  Automatizou e agilizou o provisionamento do SO dos PCs, principalmente nos laboratórios
Wapt | Permitiu a instalação de software remotamente e de forma automática, com flexibilidade (reduz necessidade de passar imagem)
Docker | Flexibilizou e simplificou nosssa processo de implantação/recuperação de novas aplicações, otimizando recursos em relação às VMs.
Puppet | Acho que tivemos ganhos parciais, principalmente nos Linux dos laboratórios, não é mesmo? 

# Ferramentas, fluxos e tecnologias para adotarmos/melhorarmos o quanto antes
Tabela de recursos fundamentais que precisaríamos adotar ou nos desenvolver:
Recurso                      | Relevância |
-----------------------------| -----------
Git e cultura de versionamento     | Acho que já usamos razoavelemente o versionamento, mas talvez possamos melhorar, embora pra isso talvez dependa de outros fluxos tais como definir ferramentas de CI/CD (Gitlab CI, Github Action, Ansible?)
GitLab   | Me parece a alternativa mais completa e acessível para nosso contexto, para ser o reposítorio de códígo principal, plataforma de CI/CD, Registry, Runner e até gestão de processos (vide Board estilo Trelho)
Github | Não pode ser descartada como plataforma auxiliar, principalmente para disponibilizarmos nossos projeto como código opensource que poderiam receber contribuições da comunidade. Fora questões de redundãncia dos dados
Ansible | Avalia-se o Ansible como boa alternativa de orquestrador e gestor de configurações pela versatilidade, com ele dá pra gerenciar desde os ativos de rede até a cloud
Logs, Monitoração e Onservabilidade | Precisamos melhorar nossa stack de monitoração e logs (Graylog, Zabbix) em número de servços monitorados e em recursos de observabilidade, que incluem tracker de erros (Prometheus), melhor visualização (Grafana).
Teste automatizados | Precisamos incluir numa pipeline de CI/CD, testes automatizados, ainda que básicos, sejam unitários, de integração ou também análise de vulnerabilidade e testes de performance.

# Outras abordagens desejáveis
Recursos ainda distantes mais que seriam fortemente desajáveis no nosso contexto.
Recurso                      | Relevância |
-----------------------------| -----------
Terraform, CloudFormation ou outros orquestradores de nuvem | Na medida que adotarmos a cloud, seria bom ter expertise nas ferramentas mais úteis.

