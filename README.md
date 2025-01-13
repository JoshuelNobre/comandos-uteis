# Comandos Úteis

## Terraform Commands

1. **Inicializar o Terraform com configuração de backend específica**  
   ```bash
   terraform init --backend-config=environment/dev/backend.tfvars
   ```  
2. **Formatar os arquivos Terraform de forma recursiva**  
   ```bash
   terraform fmt --recursive
   ```  
3. **Aplicar configurações com auto-aprovação**  
   ```bash
   terraform apply --auto-approve --var-file=environment/dev/terraform.tfvars
   ```  
4. **Destruir configurações com auto-aprovação**  
   ```bash
   terraform destroy --auto-approve --var-file=environment/dev/terraform.tfvars
   ```  
---

## Linux Commands

1. **Procurar algo independente do lugar**  
   ```bash
   find / -iname **openfeign**
   ```  
2. **Criar vários arquivos simultaneamente**  
   ```bash
   touch {variables,providers,outputs,backend}.tf
   ```  
3. **Criar vários arquivos em uma pasta específica**  
   ```bash
   touch environment/prod/{backend,terraform}.tfvars
   ```

---

## AWS Commands

1. **Adicionar o cluster EKS ao contexto do kubeconfig**  
   ```bash
   aws eks --region us-east-1 update-kubeconfig --name linuxtips-cluster
   ```
   
---

## Kubernetes Commands

1. **Lista todos os contextos disponíveis no kubeconfig**  
   ```bash
   kubectl config get-contexts
   ```
2. **Exibe o contexto ativo no momento**  
   ```bash
   kubectl config current-context
   ```
3. **Troca para o contexto especificado**  
   ```bash
   kubectl config use-context <context-name>
   ```  
