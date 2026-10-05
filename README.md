# DIO Desafio Gerenciando Politicas em Acessos Azure

Este guia apresenta conceitos fundamentais relacionados à governança e gerenciamento de políticas de acesso no **Microsoft Azure**, abordando o **Portal de Confiança do Serviço**, bloqueios de recursos, **Microsoft Purview Accounts** e **Azure Policy**.

---

## 🔒 Portal de Confiança do Serviço (Service Trust Portal)

🔗 [Service Trust Portal](https://servicetrust.microsoft.com/)

O **Portal de Confiança do Serviço** é a plataforma da Microsoft que disponibiliza informações sobre:
- **Certificados**: ISO 27001, SOC, GDPR, entre outros.
- **Regulamentos**: Documentação de conformidade com legislações globais.
- **Padrões**: Normas de segurança e privacidade aplicadas aos serviços Microsoft.

👉 Ele é essencial para equipes de **compliance e auditoria**, pois centraliza relatórios e certificações que comprovam a conformidade dos serviços em nuvem.

---

## 🛡️ Bloqueio de Deleção em Grupos de Recursos

O **Resource Lock** é uma funcionalidade que protege recursos contra exclusão ou alteração acidental.

- **Bloqueio de exclusão aplicado em um Grupo de Recursos**:
  - Impede que o grupo ou qualquer recurso dentro dele seja removido.
  - Mesmo usuários com permissões elevadas não conseguem excluir até que o bloqueio seja removido.

- **Implicações na movimentação de recursos**:
  - Se um recurso estiver em um grupo com bloqueio de exclusão, **não poderá ser movido para outro grupo** até que o bloqueio seja retirado.
  - Isso garante maior segurança contra mudanças não planejadas.

---

## 📊 Microsoft Purview Accounts

O **Microsoft Purview** é a solução de **Governança, Risco e Conformidade (GRC)** da Microsoft.

- **Purview Accounts** permitem:
  - Catalogar e classificar dados em ambientes híbridos e multicloud.
  - Monitorar conformidade regulatória.
  - Obter uma **visão unificada dos dados** corporativos.
  - Aplicar políticas de acesso e proteção de informações sensíveis.

👉 É uma ferramenta estratégica para empresas que precisam atender requisitos de **LGPD, GDPR** e outras normas de proteção de dados.

---

## 📜 Azure Policy

O **Azure Policy** é o serviço que permite criar, atribuir e gerenciar políticas para garantir conformidade dos recursos.

- **Funcionalidades principais**:
  - Definir regras (ex.: "Todas as VMs devem estar na região Brazil South").
  - Aplicar automaticamente configurações de segurança.
  - Auditar recursos existentes e identificar não conformidades.
  - Integrar com **Azure Blueprints** para governança em larga escala.

- **Exemplo prático**:
  - Criar uma política que **impede a criação de VMs sem criptografia de disco**.
  - Monitorar e corrigir automaticamente recursos fora do padrão.

---

## 📌 Conclusão

Gerenciar políticas de acesso no Azure envolve:
- Usar o **Service Trust Portal** para validar conformidade e certificações.
- Aplicar **Resource Locks** para proteger contra exclusão ou movimentação acidental.
- Utilizar **Microsoft Purview Accounts** para governança e conformidade de dados.
- Configurar **Azure Policy** para garantir que todos os recursos sigam padrões corporativos e regulatórios.

Essas práticas fortalecem a **segurança, governança e conformidade** em ambientes de nuvem corporativos.

