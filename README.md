
# Phishing para Captura de Senhas do Facebook

### Ferramentas Utilizadas
- **Kali Linux**: Distribuição Linux voltada para testes de penetração e segurança.
- **setoolkit**: Ferramenta utilizada para realizar ataques de engenharia social, como phishing.

### Etapas do Ataque de Phishing

1. **Acesso root**:
   Inicie o Kali Linux com privilégios de root para executar ferramentas administrativas:
   ```bash
   sudo su
   ```

2. **Iniciando o SEToolkit**:
   Execute a ferramenta de phishing SEToolkit:
   ```bash
   setoolkit
   ```

3. **Escolhendo o tipo de ataque**:
   O primeiro passo é selecionar o tipo de ataque de **Social-Engineering** (Engenharia Social), que foca na manipulação de vítimas:
   - Selecione **Social-Engineering Attacks**.

4. **Escolhendo o vetor de ataque**:
   - Selecione **Web Site Attack Vectors** para atacar a página de login de um site.
   - Escolha **Credential Harvester Attack Method** para capturar credenciais.
   
5. **Clonando o site**:
   - Selecione **Site Cloner** para clonar o site alvo (neste caso, o Facebook).
   - Isso cria uma página falsa de login do Facebook que parece idêntica à original.

6. **Obtendo o endereço IP da máquina**:
   - Use o comando `ifconfig` para descobrir o endereço IP da máquina onde o phishing será hospedado.

7. **URL para o clone**:
   Acesse o site original (por exemplo, **http://www.facebook.com**) e configure o phishing para capturar as credenciais da vítima.

### Resultados

![Alt text](./passwd.png "Captura de senhas")

### O que Aprendi

- **Phishing**: Aprendi a realizar ataques de phishing usando o **SEToolkit**, que cria páginas falsas para capturar informações sensíveis dos usuários.
- **Engenharia Social**: Através deste exercício, entendi como a engenharia social pode ser usada para enganar usuários e coletar dados privados, como senhas.
- **Uso de Kali Linux**: Familiarizei-me com o **Kali Linux**, uma ferramenta para testes de penetração, e como usá-la para executar ataques simulados de phishing de forma controlada.
- **Importância da Ética**: Embora o phishing seja uma técnica eficaz de cibersegurança, é essencial entender que esse conhecimento deve ser usado para melhorar a segurança e não para explorar ou prejudicar pessoas. Realizar testes somente em ambientes controlados e com autorização é uma prática ética e legal.

---

