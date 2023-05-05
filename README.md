<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
  </head>
  <body>
    <h1>Configuração de ambiente de desenvolvimento com Vagrant e Ansible</h1>
    <p>Este repositório contém exemplos de como criar e configurar máquinas virtuais usando o Vagrant e o Ansible.</p>

    <h2>Tecnologias utilizadas</h2>
    <ul>
      <li><img src="https://www.vectorlogo.zone/logos/vagrantup/vagrantup-icon.svg" alt="Vagrant" width="16" height="16"> Vagrant</li>
      <li><img src="https://www.vectorlogo.zone/logos/ansible/ansible-icon.svg" alt="Ansible" width="16" height="16"> Ansible</li>
    </ul>

    <h2>Como utilizar</h2>
    <ol>
      <li>Instale o Vagrant e o VirtualBox na sua máquina. Consulte a documentação oficial para saber como instalar em seu sistema operacional:</li>
        <ul>
          <li><a href="https://www.vagrantup.com/docs/installation/">Vagrant</a></li>
          <li><a href="https://www.virtualbox.org/manual/ch02.html">VirtualBox</a></li>
        </ul>
      <li>Clone este repositório:</li>
        <pre><code>git clone https://github.com/seu-usuario/configuracao-ambiente-dev.git</code></pre>
      <li>Crie a máquina virtual para o ambiente de desenvolvimento:</li>
        <pre><code>cd ambiente-dev
vagrant up</code></pre>
      <li>Crie a máquina virtual para o ambiente de produção:</li>
        <pre><code>cd ambiente-prod
vagrant up</code></pre>
      <li>Execute o playbook do Ansible para configurar as máquinas:</li>
        <pre><code>cd ambiente-dev
ansible-playbook -i inventories/development playbook.yml</code></pre>
        <pre><code>cd ambiente-prod
ansible-playbook -i inventories/production playbook.yml</code></pre>
    </ol>

    <h2>Referências</h2>
    <ul>
      <li><a href="https://www.vagrantup.com/docs/">Documentação do Vagrant</a></li>
      <li><a href="https://docs.ansible.com/">Documentação do Ansible</a></li>
    </ul>
  </body>
</html>
