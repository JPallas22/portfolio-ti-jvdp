# Projeto: Padronização e Deploy de Ambiente Corporativo em Larga Escala

## Contexto
A 11ª Brigada de Infantaria Mecanizada recebeu 25 novos computadores provenientes do escalão superior (CITEx), demandando preparação e entrega rápida aos usuários finais.

O cenário exigia padronização do ambiente, garantindo consistência, segurança e agilidade no processo de implantação.

---

## Problema
- Necessidade de configurar múltiplas máquinas em curto prazo
- Risco de inconsistência entre ambientes
- Alto tempo de setup manual
- Dependência de configurações individuais

---

## Solução
Implementação de um processo de padronização baseado em imagem de sistema (ISO), permitindo replicação rápida e consistente do ambiente.

### Fluxo operacional:

1. Recolhimento dos equipamentos dos usuários, evitando conflitos de hostname  
2. Backup completo dos dados em HD externo identificado  
3. Inicialização via pen drive bootável com Acronis  
4. Aplicação da imagem padrão do Windows 11  
5. Configuração individual pós-instalação:
   - Alteração de hostname  
   - Sincronização com servidor NTP  
   - Atualização do antivírus  
   - Execução de Windows Update  
   - Restauração dos dados do usuário  

6. Aplicação de etiqueta patrimonial e lacre de segurança  
7. Atualização dos registros do parque computacional  
8. Entrega ao usuário final  

---

## Tecnologias e Ferramentas
- Acronis (deploy de imagem)
- Windows 11
- HD externo
- Pen drive bootável
- Xen Orchestra (preparação da imagem)
- Kaspersky (proteção de endpoints)

---

## Resultados
- Padronização completa de 25 máquinas
- Redução significativa no tempo de implantação
- Ambiente consistente e escalável
- Melhoria direta na produtividade dos usuários
- Otimização de recursos com reaproveitamento de componentes

---

## Aprendizados
- Padronização é essencial para escala
- Automação reduz tempo e erro humano
- Planejamento prévio impacta diretamente na eficiência operacional

---

## Possíveis melhorias
- Implementação de deploy via rede (PXE)
- Criação de scripts automatizados pós-instalação
- Integração com ferramentas de gerenciamento centralizado
