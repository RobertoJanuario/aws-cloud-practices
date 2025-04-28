Descrição do Projeto
O objetivo desse projeto foi criar um alarme no Cloudwatch que avisasse via email quando a utilização de cpu de uma instância EC2 chegasse a 50%.
A instância criada foi uma t2 micro (free tier), utilizando AMI Linux 2023. Foi utilizado um teste de stress para fazer com que a utilização de cpu chegasse a 50%.

Ferramentas utilizadas: EC2, CloudWatch, SSH.

Funcionamento: Um alarme é configurado no CloudWatch para monitorar a utilização da CPU da instância EC2 e é disparado quando o uso da CPU atinge 50%.

 Prints do Projeto

Etapa	Descrição	Imagem
1	Instância EC2 criada e configurada	| [ec2 instance] https://github.com/RobertoJanuario/aws-cloud-practices/blob/master/instancia.png
2	Conexão SSH estabelecida com a EC2 | [ssh connection] https://github.com/RobertoJanuario/aws-cloud-practices/blob/master/login_ssh.png
3	CPU sendo estressada para disparar o alarme	[stress] https://github.com/RobertoJanuario/aws-cloud-practices/blob/master/rodando_stress.png
4	Alarme configurado e monitorando a instância	[alarm] https://github.com/RobertoJanuario/aws-cloud-practices/blob/master/alarme_aws.png
5	Alarme disparado devido ao alto uso de CPU	[email alarm} https://github.com/RobertoJanuario/aws-cloud-practices/blob/master/alarme_email.png

Não se trata de um tutorial, mas sim de uma aplicação prática da ferramenta para monitoramento.
