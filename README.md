# arquiteturacontainers

## Requirements

Terraform
Inframap
Graphviz

## Comandos

Operacao terraform
terraform fmt --recursive
terraform init -backend-config=environment/dev/backend.tfvars
terraform validate

Criacao de infra
terraform apply -auto-approve -var-file=environment/dev/terraform.tfvars

Destruicao de infra
terraform destroy -auto-approve -var-file=environment/dev/terraform.tfvars

Criacao de diagrama
inframap generate ./ --raw | dot -Tpng > diagrama.png

## Estrutura
![Estrutura terraform](diagrama.png)

<!-- BEGIN_TF_DOCS -->

<!-- END_TF_DOCS -->